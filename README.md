
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>ملف الإنجاز المهني - المعلمة سارة الخالدي</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Cairo', Tahoma, Geneva, Verdana, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }
        
        :root {
            --primary-blue: #4361ee;
            --secondary-blue: #3a0ca3;
            --light-blue: #4cc9f0;
            --accent-pink: #f72585;
            --light-pink: #ff9ebb;
            --cream: #fff8f0;
            --light-cream: #fffcf8;
            --soft-gray: #f8f9fa;
            --text-dark: #2b2d42;
            --text-light: #6c757d;
            --gradient-primary: linear-gradient(135deg, var(--primary-blue), #7209b7);
            --gradient-secondary: linear-gradient(135deg, var(--light-blue), #3a0ca3);
            --gradient-accent: linear-gradient(135deg, var(--accent-pink), #ff9ebb);
            --gradient-light: linear-gradient(135deg, #ffffff, var(--cream));
        }
        
        body {
            background: linear-gradient(135deg, #ffffff 0%, var(--cream) 50%, #f0f4ff 100%);
            color: var(--text-dark);
            line-height: 1.7;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
            -webkit-text-size-adjust: 100%;
        }
        
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(67, 97, 238, 0.08) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(76, 201, 240, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(247, 37, 133, 0.03) 0%, transparent 50%);
            z-index: -1;
            pointer-events: none;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 15px;
            width: 100%;
        }
        
        /* الهيدر المشرق */
        .navbar {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--secondary-blue) 100%);
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(67, 97, 238, 0.2);
            height: auto;
            min-height: 80px;
            border-bottom: 4px solid var(--accent-pink);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            padding: 10px 0;
        }
        
        .nav-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px 15px;
            gap: 15px;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-weight: 700;
            font-size: 1.2rem;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            width: 100%;
            justify-content: center;
            text-align: center;
        }
        
        .logo-icon {
            background: linear-gradient(135deg, var(--primary-blue), var(--accent-pink));
            width: 50px;
            height: 50px;
            min-width: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 15px rgba(67, 97, 238, 0.3);
            border: 2px solid rgba(255, 255, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .logo-icon i {
            font-size: 1.5rem;
            z-index: 1;
            color: white;
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
            flex: 1;
        }
        
        .logo-title {
            font-size: 1.4rem;
            background: linear-gradient(to right, #ffffff, var(--light-pink));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 700;
            line-height: 1.3;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        
        .logo-subtitle {
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 300;
            margin-top: 3px;
        }
        
        /* شريط الأيقونات الملون */
        .nav-icons-container {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 8px;
            width: 100%;
            overflow: hidden;
            max-width: 100%;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .nav-icons {
            display: flex;
            gap: 5px;
            overflow-x: auto;
            scrollbar-width: none;
            padding: 5px;
            -webkit-overflow-scrolling: touch;
            scroll-behavior: smooth;
        }
        
        .nav-icons::-webkit-scrollbar {
            display: none;
        }
        
        .nav-icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 8px 12px;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            text-decoration: none;
            color: white;
            border-radius: 12px;
            min-width: 70px;
            height: 50px;
            position: relative;
            overflow: hidden;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
            flex-shrink: 0;
            touch-action: manipulation;
        }
        
        .nav-icon::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.2), transparent);
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .nav-icon:hover, .nav-icon.active {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
        }
        
        .nav-icon.active {
            background: rgba(247, 37, 133, 0.3);
            box-shadow: 0 6px 15px rgba(247, 37, 133, 0.2);
        }
        
        .nav-icon:hover::before {
            opacity: 1;
        }
        
        .nav-icon i {
            font-size: 1.1rem;
            margin-bottom: 4px;
            z-index: 1;
        }
        
        .nav-icon span {
            font-size: 0.7rem;
            font-weight: 600;
            white-space: nowrap;
            z-index: 1;
        }
        
        /* المحتوى الرئيسي المشرق */
        .main-content {
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.95), rgba(255, 248, 240, 0.9));
            border-radius: 20px;
            box-shadow: 
                0 10px 30px rgba(67, 97, 238, 0.1),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            margin-top: 20px;
            margin-bottom: 20px;
            padding: 25px 20px;
            min-height: auto;
            border: 1px solid rgba(67, 97, 238, 0.1);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }
        
        .main-content::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-blue), var(--accent-pink));
        }
        
        .section {
            display: none;
            animation: fadeInUp 0.5s ease;
        }
        
        .section.active {
            display: block;
        }
        
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .section-title {
            color: var(--secondary-blue);
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid rgba(67, 97, 238, 0.2);
            position: relative;
            font-size: 1.6rem;
            font-weight: 700;
            line-height: 1.3;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -2px;
            right: 0;
            width: 80px;
            height: 3px;
            background: linear-gradient(90deg, var(--primary-blue), var(--accent-pink));
            border-radius: 2px;
        }
        
        /* قسم نبذة عني المشرق */
        .about-section {
            max-width: 100%;
            margin: 0 auto;
        }
        
        .about-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 18px;
            padding: 25px 20px;
            margin-bottom: 25px;
            border-left: 5px solid var(--accent-pink);
            box-shadow: 
                0 10px 25px rgba(67, 97, 238, 0.1),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            animation: fadeIn 0.5s ease;
            position: relative;
            overflow: hidden;
        }
        
        .about-card::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, rgba(67, 97, 238, 0.05) 0%, transparent 70%);
            z-index: 0;
        }
        
        .about-header {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 25px;
            gap: 20px;
            position: relative;
            z-index: 1;
            text-align: center;
        }
        
        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary-blue), var(--accent-pink));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
            box-shadow: 
                0 6px 20px rgba(67, 97, 238, 0.2),
                inset 0 3px 6px rgba(255, 255, 255, 0.3);
            border: 3px solid rgba(255, 255, 255, 0.3);
        }
        
        .about-info h3 {
            color: var(--secondary-blue);
            margin-bottom: 12px;
            font-size: 1.6rem;
            font-weight: 700;
            line-height: 1.3;
        }
        
        .about-info p {
            color: var(--text-dark);
            line-height: 1.6;
            margin-bottom: 10px;
            font-size: 1rem;
        }
        
        .highlight {
            color: var(--accent-pink);
            font-weight: 600;
        }
        
        .about-details {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .detail-item {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.9), rgba(240, 244, 255, 0.8));
            border-radius: 15px;
            padding: 20px;
            border-top: 3px solid var(--primary-blue);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.1);
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .detail-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(67, 97, 238, 0.15);
        }
        
        .detail-item h4 {
            color: var(--secondary-blue);
            margin-bottom: 12px;
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.2rem;
        }
        
        .detail-item h4 i {
            color: var(--accent-pink);
            background: rgba(247, 37, 133, 0.1);
            width: 35px;
            height: 35px;
            min-width: 35px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
        }
        
        .detail-item p {
            color: var(--text-dark);
            line-height: 1.6;
            font-size: 1rem;
        }
        
        /* المقدمة - ألوان مشرقة */
        .intro-section {
            max-width: 100%;
            margin: 0 auto;
        }
        
        .intro-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(255, 248, 240, 0.9));
            border-radius: 15px;
            padding: 20px;
            margin-bottom: 20px;
            border-right: 3px solid var(--accent-pink);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.1);
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease;
        }
        
        .intro-card:hover {
            transform: translateY(-3px);
        }
        
        .intro-card h3 {
            color: var(--secondary-blue);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            font-size: 1.3rem;
            line-height: 1.3;
        }
        
        .intro-card h3 i {
            color: var(--primary-blue);
            background: rgba(67, 97, 238, 0.1);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            margin-top: 2px;
        }
        
        .intro-card p {
            color: var(--text-dark);
            line-height: 1.6;
            margin-bottom: 12px;
            font-size: 1rem;
        }
        
        /* السيرة المهنية - ألوان مشرقة */
        .bio-grid {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .bio-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(67, 97, 238, 0.1);
            text-align: center;
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .bio-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-blue), var(--accent-pink));
        }
        
        .bio-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(67, 97, 238, 0.15);
        }
        
        .bio-card i {
            font-size: 2.5rem;
            color: var(--accent-pink);
            margin-bottom: 15px;
            background: rgba(247, 37, 133, 0.1);
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-left: auto;
            margin-right: auto;
        }
        
        .bio-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 12px;
            font-size: 1.3rem;
            font-weight: 600;
        }
        
        .bio-card p {
            color: var(--text-dark);
            font-size: 1rem;
            line-height: 1.6;
        }
        
        /* التخطيط للتدريس - ألوان مشرقة */
        .planning-grid {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .plan-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border-top: 5px solid var(--primary-blue);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.1);
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease;
        }
        
        .plan-card:hover {
            transform: translateY(-5px);
        }
        
        .plan-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            font-size: 1.3rem;
            line-height: 1.3;
        }
        
        .plan-card h4 i {
            color: var(--primary-blue);
            background: rgba(67, 97, 238, 0.1);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            margin-top: 2px;
        }
        
        .plan-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .plan-card li {
            padding: 10px 0;
            border-bottom: 1px solid rgba(67, 97, 238, 0.1);
            position: relative;
            padding-right: 25px;
            color: var(--text-dark);
            font-size: 1rem;
            line-height: 1.5;
        }
        
        .plan-card li:before {
            content: "•";
            color: var(--accent-pink);
            font-size: 1.5rem;
            position: absolute;
            right: 0;
            top: 8px;
        }
        
        /* استراتيجيات التدريس - ألوان مشرقة */
        .strategy-container {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .strategy-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(67, 97, 238, 0.1);
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .strategy-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 100%;
            background: linear-gradient(180deg, var(--primary-blue), var(--accent-pink));
        }
        
        .strategy-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(67, 97, 238, 0.15);
        }
        
        .strategy-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 12px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            font-size: 1.3rem;
            line-height: 1.3;
        }
        
        .strategy-card h4 i {
            color: var(--primary-blue);
            background: rgba(67, 97, 238, 0.1);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            margin-top: 2px;
        }
        
        .strategy-card p {
            color: var(--text-dark);
            font-size: 1rem;
            line-height: 1.6;
        }
        
        /* التقنية والمبادرات - ألوان مشرقة */
        .tech-grid {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .tech-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border-left: 5px solid var(--accent-pink);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.1);
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease;
        }
        
        .tech-card:hover {
            transform: translateY(-5px);
        }
        
        .tech-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 15px;
            font-size: 1.3rem;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(67, 97, 238, 0.2);
        }
        
        .tech-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .tech-card li {
            padding: 10px 0;
            color: var(--text-dark);
            position: relative;
            padding-right: 25px;
            border-bottom: 1px solid rgba(67, 97, 238, 0.1);
            font-size: 1rem;
            line-height: 1.5;
        }
        
        .tech-card li:before {
            content: "✓";
            color: var(--accent-pink);
            position: absolute;
            right: 0;
            top: 10px;
            font-weight: bold;
            font-size: 1.1rem;
        }
        
        /* التعلم الذاتي - ألوان مشرقة */
        .self-learning {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .learning-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease;
        }
        
        .learning-card:hover {
            transform: translateY(-5px);
        }
        
        .learning-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            font-size: 1.3rem;
            line-height: 1.3;
        }
        
        .learning-card h4 i {
            color: var(--primary-blue);
            background: rgba(67, 97, 238, 0.1);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            margin-top: 2px;
        }
        
        .learning-card p {
            color: var(--text-dark);
            line-height: 1.6;
            font-size: 1rem;
        }
        
        /* التقييم الذاتي - ألوان مشرقة */
        .assessment-container {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin-top: 25px;
        }
        
        .assessment-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 15px;
            padding: 20px;
            border-top: 5px solid;
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.1);
            border: 1px solid rgba(67, 97, 238, 0.1);
            transition: transform 0.3s ease;
        }
        
        .strength {
            border-top-color: var(--primary-blue);
        }
        
        .improvement {
            border-top-color: var(--accent-pink);
        }
        
        .plan {
            border-top-color: var(--light-blue);
        }
        
        .assessment-card:hover {
            transform: translateY(-5px);
        }
        
        .assessment-card h4 {
            color: var(--secondary-blue);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            font-size: 1.3rem;
            line-height: 1.3;
        }
        
        .assessment-card h4 i {
            background: rgba(67, 97, 238, 0.1);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.1rem;
            margin-top: 2px;
        }
        
        .strength h4 i {
            color: var(--primary-blue);
        }
        
        .improvement h4 i {
            color: var(--accent-pink);
        }
        
        .plan h4 i {
            color: var(--light-blue);
        }
        
        .assessment-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .assessment-card li {
            padding: 10px 0;
            color: var(--text-dark);
            position: relative;
            padding-right: 25px;
            border-bottom: 1px solid rgba(67, 97, 238, 0.1);
            font-size: 1rem;
            line-height: 1.5;
        }
        
        .assessment-card li:before {
            content: "•";
            color: var(--accent-pink);
            position: absolute;
            right: 0;
            top: 10px;
            font-size: 1.5rem;
        }
        
        /* الخاتمة - ألوان مشرقة */
        .conclusion-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.95), rgba(240, 244, 255, 0.9));
            border-radius: 18px;
            padding: 25px 20px;
            margin-top: 30px;
            text-align: center;
            border: 1px solid rgba(67, 97, 238, 0.1);
            box-shadow: 0 10px 25px rgba(67, 97, 238, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .conclusion-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-blue), var(--accent-pink));
        }
        
        .conclusion-card h3 {
            color: var(--secondary-blue);
            margin-bottom: 20px;
            font-size: 1.6rem;
            line-height: 1.3;
        }
        
        .conclusion-card p {
            color: var(--text-dark);
            line-height: 1.6;
            margin-bottom: 15px;
            font-size: 1rem;
            text-align: right;
        }
        
        /* تذييل الصفحة - ألوان مشرقة */
        .footer {
            text-align: center;
            padding: 20px 15px;
            margin-top: 20px;
            color: var(--text-light);
            border-top: 1px solid rgba(67, 97, 238, 0.1);
            font-size: 0.85rem;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 12px;
            margin-bottom: 15px;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            line-height: 1.5;
        }
        
        /* تحسينات للشاشات المتوسطة والكبيرة */
        @media (min-width: 576px) {
            .container {
                padding: 0 20px;
            }
            
            .nav-icon {
                min-width: 80px;
                padding: 10px 15px;
            }
            
            .nav-icon span {
                font-size: 0.75rem;
            }
            
            .logo-title {
                font-size: 1.5rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .about-header {
                flex-direction: row;
                text-align: right;
                align-items: center;
            }
            
            .avatar {
                width: 140px;
                height: 140px;
                font-size: 3.5rem;
            }
            
            .about-info h3 {
                font-size: 1.8rem;
            }
        }
        
        @media (min-width: 768px) {
            .navbar {
                height: 100px;
                padding: 0;
            }
            
            .nav-container {
                flex-direction: row;
                justify-content: space-between;
                padding: 0 30px;
                height: 100px;
            }
            
            .logo {
                width: auto;
                justify-content: flex-start;
            }
            
            .nav-icons-container {
                width: auto;
                max-width: 70%;
            }
            
            .logo-title {
                font-size: 1.6rem;
            }
            
            .logo-subtitle {
                font-size: 1rem;
            }
            
            .main-content {
                padding: 35px 30px;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .about-details {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .bio-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .planning-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .strategy-container {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .tech-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .self-learning {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
            
            .assessment-container {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 25px;
            }
        }
        
        @media (min-width: 992px) {
            .nav-icons-container {
                max-width: 75%;
            }
            
            .nav-icon {
                min-width: 85px;
                padding: 10px 18px;
            }
            
            .nav-icon span {
                font-size: 0.8rem;
            }
            
            .about-details {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .bio-grid {
                grid-template-columns: repeat(4, 1fr);
            }
            
            .planning-grid {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .strategy-container {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .tech-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .assessment-container {
                grid-template-columns: repeat(3, 1fr);
            }
        }
        
        @media (min-width: 1200px) {
            .nav-icon {
                min-width: 90px;
            }
            
            .logo-title {
                font-size: 1.8rem;
            }
            
            .planning-grid {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .strategy-container {
                grid-template-columns: repeat(4, 1fr);
            }
        }
        
        /* تأثيرات إضافية */
        .fade-in-element {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.5s ease, transform 0.5s ease;
        }
        
        .fade-in-element.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* تأثيرات متحركة */
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-5px); }
            100% { transform: translateY(0px); }
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        /* تحسين الأداء للجوال */
        .no-select {
            -webkit-touch-callout: none;
            -webkit-user-select: none;
            -khtml-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
        }
    </style>
</head>
<body class="no-select">
    <!-- الهيدر المشرق -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <div class="logo-icon pulse">
                    <i class="fas fa-chalkboard-teacher"></i>
                </div>
                <div class="logo-text">
                    <div class="logo-title">ملف الإنجاز المهني</div>
                    <div class="logo-subtitle">المعلمة: سارة الخالدي</div>
                </div>
            </div>
            
            <div class="nav-icons-container">
                <div class="nav-icons">
                    <a href="#" class="nav-icon active" data-target="about">
                        <i class="fas fa-user-circle"></i>
                        <span>نبذة عني</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="intro">
                        <i class="fas fa-home"></i>
                        <span>المقدمة</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="bio">
                        <i class="fas fa-user-tie"></i>
                        <span>السيرة</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="planning">
                        <i class="fas fa-calendar-alt"></i>
                        <span>التخطيط</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="strategies">
                        <i class="fas fa-chalkboard"></i>
                        <span>استراتيجيات</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="evaluation">
                        <i class="fas fa-clipboard-check"></i>
                        <span>التقويم</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="technology">
                        <i class="fas fa-laptop"></i>
                        <span>التقنية</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="initiatives">
                        <i class="fas fa-lightbulb"></i>
                        <span>المبادرات</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="students">
                        <i class="fas fa-users"></i>
                        <span>الطلاب</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="self-learning">
                        <i class="fas fa-book"></i>
                        <span>التعلم الذاتي</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="assessment">
                        <i class="fas fa-chart-line"></i>
                        <span>التقييم</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="conclusion">
                        <i class="fas fa-flag"></i>
                        <span>الخاتمة</span>
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- المحتوى الرئيسي المشرق -->
    <div class="container">
        <div class="main-content">
            <!-- نبذة عني -->
            <section id="about" class="section active">
                <h2 class="section-title">نبذة عني</h2>
                <div class="about-section">
                    <div class="about-card">
                        <div class="about-header">
                            <div class="avatar floating">
                                <i class="fas fa-chalkboard-teacher"></i>
                            </div>
                            <div class="about-info">
                                <h3>سارة خويتم عبدالجبار الخالدي</h3>
                                <p><span class="highlight">التخصص:</span> رياضيات وإحصاء</p>
                                <p><span class="highlight">المهنة:</span> معلمة رياضيات للمرحلة الابتدائية</p>
                                <p><span class="highlight">الخبرة:</span> 4 سنوات في القطاع الخاص</p>
                                <p>معلمة متخصصة في تدريس الرياضيات للمرحلة الابتدائية، أمتلك شغفاً كبيراً في تطوير مهارات الطلاب واستخدام أساليب تربوية حديثة.</p>
                            </div>
                        </div>
                        
                        <div class="about-details">
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-heartbeat"></i> فلسفتي التعليمية</h4>
                                <p>أؤمن بأن التعليم عملية إبداعية تهدف إلى تنمية التفكير النقدي والإبداعي لدى الطلاب، وليس مجرد نقل للمعرفة.</p>
                            </div>
                            
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-rocket"></i> منهجي في التدريس</h4>
                                <p>أعتمد على استراتيجيات تعليمية متنوعة تراعي الفروق الفردية بين الطلاب، مع التركيز على التعلم النشط والتطبيقات العملية.</p>
                            </div>
                            
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-trophy"></i> إنجازاتي التربوية</h4>
                                <p>حصلت على تقدير "المعلم المتميز" مرتين، وساهمت في رفع معدل نجاح طلابي في اختبارات الرياضيات بنسبة 40%.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
            <!-- المقدمة -->
            <section id="intro" class="section">
                <h2 class="section-title">المقدمة</h2>
                <div class="intro-section">
                    <div class="intro-card fade-in-element">
                        <h3><i class="fas fa-question-circle"></i> رؤيتي التعليمية</h3>
                        <p>أتطلع إلى إنشاء جيل من الطلاب المتمكنين في الرياضيات، القادرين على تطبيق المفاهيم الرياضية في حياتهم اليومية.</p>
                    </div>
                    
                    <div class="intro-card fade-in-element">
                        <h3><i class="fas fa-bullseye"></i> رسالتي التربوية</h3>
                        <p>تقديم تعليم رياضي متميز يلبي احتياجات جميع الطلاب، باستخدام استراتيجيات تدريس مبتكرة وتقنيات تعليمية حديثة.</p>
                    </div>
                    
                    <div class="intro-card fade-in-element">
                        <h3><i class="fas fa-star"></i> قيمي التعليمية</h3>
                        <p>الإبداع، التميز، العدالة، التعاون، والمسؤولية. أؤمن بأهمية تقديم تعليم عالي الجودة لجميع الطلاب.</p>
                    </div>
                </div>
            </section>
            
            <!-- السيرة المهنية المختصرة -->
            <section id="bio" class="section">
                <h2 class="section-title">السيرة المهنية المختصرة</h2>
                <div class="bio-grid">
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-graduation-cap"></i>
                        <h4>المؤهل العلمي</h4>
                        <p>بكالوريوس تربية - تخصص رياضيات وإحصاء - جامعة الطائف - بتقدير امتياز</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-book"></i>
                        <h4>التخصص الدقيق</h4>
                        <p>معلمة رياضيات للمرحلة الابتدائية - متخصصة في تدريس الرياضيات التطبيقية والتفاعلية</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-briefcase"></i>
                        <h4>المسيرة المهنية</h4>
                        <p>4 سنوات في القطاع الخاص - تدريس الرياضيات لطلاب المرحلة الابتدائية في مدارس النخبة الخاصة</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-chalkboard"></i>
                        <h4>المهارات التخصصية</h4>
                        <p>تصميم مناهج رياضية تفاعلية - استخدام تقنيات التعليم الحديثة - تقييم وتطوير الأداء التعليمي</p>
                    </div>
                </div>
            </section>
            
            <!-- التخطيط للتدريس -->
            <section id="planning" class="section">
                <h2 class="section-title">التخطيط للتدريس</h2>
                <div class="planning-grid">
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-file-alt"></i> تحضير درس متكامل</h4>
                        <ul>
                            <li>تحليل المحتوى وتحديد الأهداف التعليمية</li>
                            <li>تصميم أنشطة تعليمية تفاعلية متنوعة</li>
                            <li>إعداد وسائل تعليمية مبتكرة وجذابة</li>
                            <li>تخطيط أساليب تقييم متنوعة</li>
                            <li>إعداد مواد إثرائية وداعمة</li>
                        </ul>
                    </div>
                    
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-calendar"></i> توزيع المنهج الدراسي</h4>
                        <ul>
                            <li>توزيع المقرر على الأسابيع الدراسية</li>
                            <li>مراعاة المناسبات والأحداث المدرسية</li>
                            <li>تخصيص أوقات للمراجعة والتقييم</li>
                            <li>التنسيق مع فريق العمل</li>
                            <li>مراعاة الفروق الفردية</li>
                        </ul>
                    </div>
                    
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-tasks"></i> خطة تطوير الأداء</h4>
                        <ul>
                            <li>تحديد أهداف تطويرية لكل فصل</li>
                            <li>تخطيط برامج تدريبية مستمرة</li>
                            <li>تصميم أنشطة تعاونية مع الزملاء</li>
                            <li>متابعة التطور المهني المستمر</li>
                            <li>توثيق التجارب الناجحة</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- استراتيجيات التدريس -->
            <section id="strategies" class="section">
                <h2 class="section-title">استراتيجيات التدريس المستخدمة</h2>
                <div class="strategy-container">
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-running"></i> التعلم النشط التفاعلي</h4>
                        <p>استخدام استراتيجيات مثل العصف الذهني، التعلم بالمشاريع، والتعلم القائم على حل المشكلات.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-users"></i> التعلم التعاوني المنظم</h4>
                        <p>تنظيم الطلاب في مجموعات تعاونية متنوعة المهام لتطوير مهارات التواصل والعمل الجماعي.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-gamepad"></i> التعليم الترفيهي</h4>
                        <p>دمج الألعاب التعليمية في العملية التعليمية مثل "سودوكو الأطفال" و"لعبة الضرب السريع".</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-lightbulb"></i> التعلم السياقي</h4>
                        <p>ربط الدروس الرياضية بحياة الطلاب اليومية من خلال أمثلة واقعية وتطبيقات عملية.</p>
                    </div>
                </div>
            </section>
            
            <!-- التقويم والاختبارات -->
            <section id="evaluation" class="section">
                <h2 class="section-title">التقويم والاختبارات</h2>
                <div class="tech-grid">
                    <div class="tech-card fade-in-element">
                        <h4>أنماط التقويم المستخدمة</h4>
                        <ul>
                            <li>التقويم التشخيصي القبلي</li>
                            <li>التقويم التكويني المستمر</li>
                            <li>التقويم الختامي النهائي</li>
                            <li>التقويم الذاتي للطلاب</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>تنويع أدوات التقويم</h4>
                        <ul>
                            <li>اختبارات تحريرية متنوعة</li>
                            <li>مشاريع عملية وتطبيقية</li>
                            <li>ملاحظات أداء صفية</li>
                            <li>ملفات إنجاز الطلاب</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>معالجة الضعف الدراسي</h4>
                        <ul>
                            <li>تحليل نتائج التقويم</li>
                            <li>تصميم برامج علاجية</li>
                            <li>تنفيذ جلسات تقوية</li>
                            <li>متابعة التقدم الأكاديمي</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>الاختبارات الإبداعية</h4>
                        <ul>
                            <li>اختبارات حل المشكلات</li>
                            <li>اختبارات المشروعات العملية</li>
                            <li>اختبارات الأداء التطبيقي</li>
                            <li>اختبارات التفكير الإبداعي</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- التقنية في التعليم -->
            <section id="technology" class="section">
                <h2 class="section-title">توظيف التقنية في التعليم</h2>
                <div class="tech-grid">
                    <div class="tech-card fade-in-element">
                        <h4>الأدوات الرقمية المتقدمة</h4>
                        <ul>
                            <li>منصة مدرستي للتعليم المدمج</li>
                            <li>برامج الرياضيات التفاعلية</li>
                            <li>تطبيقات الواقع المعزز</li>
                            <li>منصات الألعاب التعليمية</li>
                            <li>برامج التخطيط الذكي</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>الاختبارات الإلكترونية</h4>
                        <ul>
                            <li>تصميم اختبارات تفاعلية</li>
                            <li>استخدام تقنيات التصحيح الآلي</li>
                            <li>إنشاء بنك أسئلة إلكتروني</li>
                            <li>تصميم أنشطة تقييم ذاتي</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>مزايا التكامل التقني</h4>
                        <ul>
                            <li>تجارب تعلم شخصية</li>
                            <li>زيادة تفاعل الطلاب</li>
                            <li>تمكين التعلم عن بعد</li>
                            <li>تحسين كفاءة التقييم</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- المبادرات -->
            <section id="initiatives" class="section">
                <h2 class="section-title">المبادرات الصفية والمدرسية</h2>
                <div class="strategy-container">
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-seedling"></i> مبادرة "رياضيات الحياة"</h4>
                        <p>ربط الرياضيات بالحياة اليومية من خلال أنشطة عملية مثل تصميم ميزانية وتحليل بيانات.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-medal"></i> مسابقة "عباقرة الرياضيات"</h4>
                        <p>مسابقة فصلية تشمل تحديات رياضية متنوعة لاكتشاف المواهب وتنمية روح المنافسة.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-hands-helping"></i> نادي "أصدقاء الرياضيات"</h4>
                        <p>نادي طلابي تطوعي يهدف إلى تعزيز حب الرياضيات ومساعدة الطلاب بعضهم بعضاً.</p>
                    </div>
                </div>
            </section>
            
            <!-- العناية بالطلاب -->
            <section id="students" class="section">
                <h2 class="section-title">العناية بالطلاب</h2>
                <div class="tech-grid">
                    <div class="tech-card fade-in-element">
                        <h4>برامج الدعم الأكاديمي</h4>
                        <ul>
                            <li>برامج علاجية فردية</li>
                            <li>جلسات تقوية مرنة</li>
                            <li>مواد تعليمية مساندة</li>
                            <li>شراكات مع أولياء الأمور</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>رعاية المتفوقين</h4>
                        <ul>
                            <li>برامج إثرائية متقدمة</li>
                            <li>مشاركة في مسابقات</li>
                            <li>فرص قيادية داخلية</li>
                            <li>تشجيع البحث العلمي</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>التعلم الشامل</h4>
                        <ul>
                            <li>أنشطة متنوعة المستويات</li>
                            <li>بدائل تعليمية متنوعة</li>
                            <li>استراتيجيات تدريس مرنة</li>
                            <li>بيئة صفية داعمة</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- التعلم الذاتي -->
            <section id="self-learning" class="section">
                <h2 class="section-title">التعلم الذاتي والتطوير المهني</h2>
                <div class="self-learning">
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-book"></i> القراءة التخصصية</h4>
                        <p>متابعة أحدث الأبحاث في تدريس الرياضيات والاطلاع على المجلات التربوية المحلية والعالمية.</p>
                    </div>
                    
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-video"></i> التدريب الإلكتروني</h4>
                        <p>الالتحاق بالدورات التدريبية عبر الإنترنت وحضور المؤتمرات الافتراضية المتخصصة.</p>
                    </div>
                    
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-graduation-cap"></i> الشهادات والاعتمادات</h4>
                        <p>الحصول على شهادات في استخدام التقنية في التعليم واستراتيجيات التعلم النشط.</p>
                    </div>
                </div>
            </section>
            
            <!-- التقييم الذاتي -->
            <section id="assessment" class="section">
                <h2 class="section-title">التقييم الذاتي والتطوير المهني</h2>
                <div class="assessment-container">
                    <div class="assessment-card strength fade-in-element">
                        <h4><i class="fas fa-check-circle"></i> نقاط القوة</h4>
                        <ul>
                            <li>تبسيط المفاهيم المعقدة</li>
                            <li>استخدام التقنيات التعليمية</li>
                            <li>بناء علاقات إيجابية</li>
                            <li>التخطيط الاستراتيجي</li>
                            <li>المرونة والتكيف</li>
                        </ul>
                    </div>
                    
                    <div class="assessment-card improvement fade-in-element">
                        <h4><i class="fas fa-tools"></i> مجالات التطوير</h4>
                        <ul>
                            <li>البحث العلمي التربوي</li>
                            <li>تحليلات البيانات التعليمية</li>
                            <li>التعلم بالمشاريع</li>
                            <li>مجتمعات التعلم العالمية</li>
                        </ul>
                    </div>
                    
                    <div class="assessment-card plan fade-in-element">
                        <h4><i class="fas fa-calendar-check"></i> خطة التطوير</h4>
                        <ul>
                            <li>ماجستير في مناهج الرياضيات</li>
                            <li>منصة تعليمية تفاعلية</li>
                            <li>دليل استراتيجيات التدريس</li>
                            <li>زيارات تبادلية للمدارس</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- الخاتمة -->
            <section id="conclusion" class="section">
                <h2 class="section-title">الخاتمة والتطلعات</h2>
                <div class="conclusion-card">
                    <h3>رحلة الإبداع التربوي المستمرة</h3>
                    <p>تمثل مسيرتي التعليمية رحلة متواصلة من التعلم والتطوير، حيث أسعى دائماً إلى تجويد ممارساتي التعليمية والارتقاء بمستوى أدائي المهني.</p>
                    <p>أتطلع إلى المساهمة الفعالة في تطوير التعليم الرياضي على مستوى المدرسة والمجتمع المحلي، من خلال تبني المبادرات التربوية المبتكرة.</p>
                    <p>أهدف إلى ترسيخ ثقافة التميز والإبداع في تدريس الرياضيات، وجعلها مادة محببة ومفهومة لجميع الطلاب.</p>
                    <div style="margin-top: 25px; padding-top: 20px; border-top: 2px solid rgba(67, 97, 238, 0.2);">
                        <p style="font-weight: 700; color: var(--secondary-blue); font-size: 1.1rem;">
                            المعلمة المتميزة<br>
                            <span style="color: var(--accent-pink); font-size: 1.2rem;">سارة خويتم الخالدي</span><br>
                            معلمة رياضيات - المرحلة الابتدائية<br>
                            ديسمبر 2023
                        </p>
                    </div>
                </div>
            </section>
        </div>
        
        <div class="footer">
            <p>© 2023 ملف الإنجاز - المعلمة سارة خويتم الخالدي</p>
            <p>جميع الحقوق محفوظة | تم التحديث في ديسمبر 2023</p>
            <div style="margin-top: 15px;">
                <i class="fas fa-envelope" style="margin: 0 10px; color: var(--accent-pink);"></i>
                <i class="fas fa-phone" style="margin: 0 10px; color: var(--primary-blue);"></i>
                <i class="fas fa-globe" style="margin: 0 10px; color: var(--light-blue);"></i>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const navIcons = document.querySelectorAll('.nav-icon');
            const sections = document.querySelectorAll('.section');
            
            // وظيفة لتحميل الأقسام
            function loadSection(targetId) {
                // إزالة النشاط من جميع الأيقونات
                navIcons.forEach(item => item.classList.remove('active'));
                
                // إضافة النشاط للأيقونة المختارة
                document.querySelector(`.nav-icon[data-target="${targetId}"]`).classList.add('active');
                
                // إخفاء جميع الأقسام
                sections.forEach(section => section.classList.remove('active'));
                
                // عرض القسم المطلوب
                const targetSection = document.getElementById(targetId);
                targetSection.classList.add('active');
                
                // تفعيل تأثيرات الظهور
                setTimeout(() => {
                    const currentFadeElements = targetSection.querySelectorAll('.fade-in-element');
                    currentFadeElements.forEach((el, index) => {
                        setTimeout(() => {
                            el.classList.add('visible');
                        }, index * 50);
                    });
                }, 100);
                
                // التمرير للنصف العلوي من الصفحة على الجوال
                if (window.innerWidth < 768) {
                    window.scrollTo({
                        top: 0,
                        behavior: 'smooth'
                    });
                }
            }
            
            // إضافة Event Listeners للأيقونات
            navIcons.forEach(icon => {
                icon.addEventListener('click', function(e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('data-target');
                    loadSection(targetId);
                });
                
                // تحسين التفاعل على الجوال
                icon.addEventListener('touchstart', function() {
                    this.style.opacity = '0.8';
                });
                
                icon.addEventListener('touchend', function() {
                    this.style.opacity = '1';
                });
            });
            
            // تفعيل تأثيرات الظهور عند التمرير
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -30px 0px'
            };
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, observerOptions);
            
            document.querySelectorAll('.fade-in-element').forEach(element => {
                observer.observe(element);
            });
            
            // تفعيل العناصر في الصفحة الأولى
            setTimeout(() => {
                document.querySelectorAll('#about .fade-in-element').forEach((el, index) => {
                    setTimeout(() => {
                        el.classList.add('visible');
                    }, index * 150);
                });
            }, 300);
            
            // تهيئة الصفحة الأولى
            loadSection('about');
        });
    </script>
</body>
</html>
