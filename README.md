<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ملف الإنجاز المهني - المعلمة سارة الخالدي</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Cairo', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary-dark: #232D3F;
            --primary-purple: #8A2BE2;
            --light-purple: #976680;
            --dark-purple: #654148;
            --accent-pink: #E75480;
            --light-gray: #C0C0C0;
            --charcoal: #36454F;
            --off-white: #F8F9FA;
            --gradient-primary: linear-gradient(135deg, var(--primary-dark), #2A0F45);
            --gradient-purple: linear-gradient(135deg, var(--primary-purple), #9370DB);
            --gradient-accent: linear-gradient(135deg, var(--accent-pink), #FF69B4);
            --gradient-header: linear-gradient(135deg, #1C1C1C 0%, #4B0082 50%, #1C1C1C 100%);
        }
        
        body {
            background: linear-gradient(135deg, #1A1A2E 0%, #2D1B47 50%, #1C0F2D 100%);
            color: var(--off-white);
            line-height: 1.7;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }
        
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(138, 43, 226, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(151, 102, 128, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(231, 84, 128, 0.08) 0%, transparent 50%);
            z-index: -1;
            pointer-events: none;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* الهيدر الموسع والاحترافي */
        .navbar {
            background: linear-gradient(135deg, #2D1B47 0%, #4A235A 50%, #2D1B47 100%);
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.5);
            height: 100px;
            display: flex;
            align-items: center;
            border-bottom: 4px solid var(--accent-pink);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 30px;
            width: 100%;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 20px;
            font-weight: 700;
            font-size: 1.4rem;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        .logo-icon {
            background: linear-gradient(135deg, var(--primary-purple), var(--accent-pink));
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 6px 20px rgba(138, 43, 226, 0.5);
            border: 2px solid rgba(255, 255, 255, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .logo-icon::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent 30%, rgba(255, 255, 255, 0.1) 50%, transparent 70%);
            animation: shine 3s infinite linear;
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        .logo-icon i {
            font-size: 1.8rem;
            z-index: 1;
            color: white;
        }
        
        .logo-text {
            display: flex;
            flex-direction: column;
        }
        
        .logo-title {
            font-size: 1.8rem;
            background: linear-gradient(to right, #fff, var(--primary-purple));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 800;
            letter-spacing: 1px;
        }
        
        .logo-subtitle {
            font-size: 1rem;
            color: var(--light-gray);
            font-weight: 300;
            margin-top: 5px;
        }
        
        /* شريط الأيقونات المميز */
        .nav-icons-container {
            background: rgba(75, 0, 130, 0.85);
            border-radius: 20px;
            padding: 8px;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 
                0 8px 32px rgba(0, 0, 0, 0.4),
                inset 0 1px 0 rgba(255, 255, 255, 0.1);
        }
        
        .nav-icons {
            display: flex;
            gap: 2px;
            overflow-x: auto;
            scrollbar-width: thin;
            scrollbar-color: var(--accent-pink) rgba(75, 0, 130, 0.5);
            padding: 4px;
        }
        
        .nav-icons::-webkit-scrollbar {
            height: 6px;
        }
        
        .nav-icons::-webkit-scrollbar-track {
            background: rgba(75, 0, 130, 0.5);
            border-radius: 10px;
        }
        
        .nav-icons::-webkit-scrollbar-thumb {
            background: var(--accent-pink);
            border-radius: 10px;
        }
        
        .nav-icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 10px 20px;
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            text-decoration: none;
            color: var(--off-white);
            border-radius: 15px;
            min-width: 95px;
            height: 56px;
            position: relative;
            overflow: hidden;
            background: rgba(90, 50, 140, 0.7);
        }
        
        .nav-icon::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(138, 43, 226, 0.3), rgba(231, 84, 128, 0.2));
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .nav-icon:hover, .nav-icon.active {
            background: rgba(138, 43, 226, 0.8);
            transform: translateY(-4px) scale(1.05);
            box-shadow: 0 8px 20px rgba(138, 43, 226, 0.5);
        }
        
        .nav-icon.active {
            background: rgba(231, 84, 128, 0.8);
            box-shadow: 0 8px 20px rgba(231, 84, 128, 0.5);
        }
        
        .nav-icon:hover::before {
            opacity: 1;
        }
        
        .nav-icon::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 0;
            height: 3px;
            background: linear-gradient(90deg, var(--primary-purple), var(--accent-pink));
            transition: width 0.4s ease;
            border-radius: 3px;
        }
        
        .nav-icon.active::after, .nav-icon:hover::after {
            width: 70%;
        }
        
        .nav-icon i {
            font-size: 1.2rem;
            margin-bottom: 6px;
            z-index: 1;
            transition: transform 0.3s ease;
        }
        
        .nav-icon:hover i {
            transform: scale(1.2);
        }
        
        .nav-icon span {
            font-size: 0.75rem;
            font-weight: 600;
            white-space: nowrap;
            z-index: 1;
            letter-spacing: 0.5px;
        }
        
        /* المحتوى الرئيسي */
        .main-content {
            background: rgba(45, 27, 71, 0.9);
            border-radius: 24px;
            box-shadow: 
                0 20px 50px rgba(0, 0, 0, 0.6),
                inset 0 1px 0 rgba(255, 255, 255, 0.1);
            margin-top: 40px;
            margin-bottom: 40px;
            padding: 40px;
            min-height: calc(100vh - 200px);
            border: 1px solid rgba(255, 255, 255, 0.05);
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
            background: linear-gradient(90deg, var(--primary-purple), var(--accent-pink));
        }
        
        .section {
            display: none;
            animation: fadeInUp 0.8s ease;
        }
        
        .section.active {
            display: block;
        }
        
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .section-title {
            color: #fff;
            margin-bottom: 35px;
            padding-bottom: 20px;
            border-bottom: 2px solid rgba(138, 43, 226, 0.3);
            position: relative;
            font-size: 2.2rem;
            font-weight: 700;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -2px;
            right: 0;
            width: 120px;
            height: 4px;
            background: linear-gradient(90deg, var(--primary-purple), var(--accent-pink));
            border-radius: 2px;
        }
        
        /* قسم نبذة عني */
        .about-section {
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .about-card {
            background: linear-gradient(145deg, rgba(74, 35, 90, 0.9), rgba(45, 27, 71, 0.9));
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 40px;
            border-left: 6px solid var(--accent-pink);
            box-shadow: 
                0 15px 35px rgba(0, 0, 0, 0.6),
                inset 0 1px 0 rgba(255, 255, 255, 0.05);
            animation: fadeIn 0.8s ease;
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
            background: radial-gradient(circle, rgba(138, 43, 226, 0.2) 0%, transparent 70%);
            z-index: 0;
        }
        
        .about-header {
            display: flex;
            align-items: center;
            margin-bottom: 30px;
            gap: 30px;
            position: relative;
            z-index: 1;
        }
        
        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary-purple), var(--accent-pink));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            box-shadow: 
                0 10px 30px rgba(138, 43, 226, 0.5),
                inset 0 4px 8px rgba(255, 255, 255, 0.2);
            border: 4px solid rgba(255, 255, 255, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .avatar::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent 30%, rgba(255, 255, 255, 0.2) 50%, transparent 70%);
            animation: shine 3s infinite linear;
        }
        
        .about-info {
            flex: 1;
        }
        
        .about-info h3 {
            color: #fff;
            margin-bottom: 15px;
            font-size: 2rem;
            font-weight: 700;
            background: linear-gradient(to right, #fff, var(--primary-purple));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .about-info p {
            color: #ddd;
            line-height: 1.8;
            margin-bottom: 12px;
            font-size: 1.05rem;
        }
        
        .highlight {
            color: var(--accent-pink);
            font-weight: 600;
        }
        
        .about-details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 30px;
            position: relative;
            z-index: 1;
        }
        
        .detail-item {
            background: rgba(90, 50, 140, 0.7);
            border-radius: 15px;
            padding: 25px;
            border-top: 4px solid var(--primary-purple);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
            border-left: 1px solid rgba(255, 255, 255, 0.05);
            border-right: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .detail-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 30px rgba(138, 43, 226, 0.4);
        }
        
        .detail-item h4 {
            color: #fff;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.3rem;
        }
        
        .detail-item h4 i {
            color: var(--accent-pink);
            background: rgba(231, 84, 128, 0.1);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .detail-item p {
            color: #ccc;
            line-height: 1.7;
        }
        
        /* مقدمة - نصف صفحة */
        .intro-section {
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .intro-card {
            background: linear-gradient(145deg, rgba(74, 35, 90, 0.9), rgba(45, 27, 71, 0.9));
            border-radius: 18px;
            padding: 30px;
            margin-bottom: 30px;
            border-right: 4px solid var(--accent-pink);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
            animation: fadeIn 0.8s ease;
            transition: transform 0.3s ease;
        }
        
        .intro-card:hover {
            transform: translateY(-5px);
        }
        
        .intro-card h3 {
            color: #fff;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.5rem;
        }
        
        .intro-card h3 i {
            color: var(--primary-purple);
            background: rgba(138, 43, 226, 0.1);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .intro-card p {
            color: #ddd;
            line-height: 1.8;
            margin-bottom: 15px;
            font-size: 1.05rem;
        }
        
        /* السيرة المهنية المختصرة */
        .bio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .bio-card {
            background: linear-gradient(145deg, rgba(90, 50, 140, 0.8), rgba(74, 35, 90, 0.8));
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .bio-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary-purple), var(--accent-pink));
        }
        
        .bio-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(138, 43, 226, 0.4);
        }
        
        .bio-card i {
            font-size: 3rem;
            color: var(--accent-pink);
            margin-bottom: 20px;
            background: rgba(231, 84, 128, 0.1);
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-left: auto;
            margin-right: auto;
        }
        
        .bio-card h4 {
            color: #fff;
            margin-bottom: 15px;
            font-size: 1.4rem;
            font-weight: 600;
        }
        
        .bio-card p {
            color: #ccc;
            font-size: 1rem;
            line-height: 1.7;
        }
        
        /* التخطيط للتدريس */
        .planning-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .plan-card {
            background: linear-gradient(145deg, rgba(90, 50, 140, 0.8), rgba(74, 35, 90, 0.8));
            border-radius: 18px;
            padding: 30px;
            border-top: 6px solid var(--primary-dark);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease;
        }
        
        .plan-card:hover {
            transform: translateY(-8px);
        }
        
        .plan-card h4 {
            color: #fff;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.4rem;
        }
        
        .plan-card h4 i {
            color: var(--primary-purple);
            background: rgba(138, 43, 226, 0.1);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .plan-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .plan-card li {
            padding: 12px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            position: relative;
            padding-right: 25px;
            color: #ddd;
            transition: color 0.3s ease;
        }
        
        .plan-card li:hover {
            color: var(--accent-pink);
        }
        
        .plan-card li:before {
            content: "•";
            color: var(--accent-pink);
            font-size: 1.8rem;
            position: absolute;
            right: 0;
            top: 10px;
        }
        
        .plan-card li:last-child {
            border-bottom: none;
        }
        
        /* استراتيجيات التدريس */
        .strategy-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .strategy-card {
            background: linear-gradient(145deg, rgba(90, 50, 140, 0.8), rgba(74, 35, 90, 0.8));
            border-radius: 18px;
            padding: 30px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
            overflow: hidden;
        }
        
        .strategy-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: linear-gradient(180deg, var(--primary-purple), var(--accent-pink));
        }
        
        .strategy-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 35px rgba(138, 43, 226, 0.4);
            border-color: var(--primary-purple);
        }
        
        .strategy-card h4 {
            color: #fff;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.4rem;
        }
        
        .strategy-card h4 i {
            color: var(--primary-purple);
            background: rgba(138, 43, 226, 0.1);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .strategy-card p {
            color: #ddd;
            font-size: 1.05rem;
            line-height: 1.7;
        }
        
        /* التقنية والمبادرات */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .tech-card {
            background: linear-gradient(145deg, rgba(90, 50, 140, 0.8), rgba(74, 35, 90, 0.8));
            border-radius: 18px;
            padding: 30px;
            border-left: 6px solid var(--accent-pink);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease;
        }
        
        .tech-card:hover {
            transform: translateY(-8px);
        }
        
        .tech-card h4 {
            color: #fff;
            margin-bottom: 20px;
            font-size: 1.4rem;
            padding-bottom: 10px;
            border-bottom: 2px solid rgba(138, 43, 226, 0.3);
        }
        
        .tech-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .tech-card li {
            padding: 12px 0;
            color: #ddd;
            position: relative;
            padding-right: 30px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            transition: color 0.3s ease;
        }
        
        .tech-card li:hover {
            color: var(--accent-pink);
        }
        
        .tech-card li:before {
            content: "✓";
            color: var(--accent-pink);
            position: absolute;
            right: 0;
            top: 12px;
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        /* التعلم الذاتي */
        .self-learning {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .learning-card {
            background: linear-gradient(145deg, rgba(45, 27, 71, 0.9), rgba(90, 50, 140, 0.8));
            border-radius: 18px;
            padding: 30px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: transform 0.3s ease;
        }
        
        .learning-card:hover {
            transform: translateY(-8px);
        }
        
        .learning-card h4 {
            color: #fff;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.4rem;
        }
        
        .learning-card h4 i {
            color: var(--primary-purple);
            background: rgba(138, 43, 226, 0.1);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .learning-card p {
            color: #ddd;
            line-height: 1.7;
        }
        
        /* التقييم الذاتي */
        .assessment-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .assessment-card {
            background: linear-gradient(145deg, rgba(90, 50, 140, 0.8), rgba(74, 35, 90, 0.8));
            border-radius: 18px;
            padding: 30px;
            border-top: 6px solid;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease;
        }
        
        .assessment-card:hover {
            transform: translateY(-8px);
        }
        
        .strength {
            border-top-color: var(--primary-purple);
        }
        
        .improvement {
            border-top-color: var(--accent-pink);
        }
        
        .plan {
            border-top-color: #9370DB;
        }
        
        .assessment-card h4 {
            color: #fff;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.4rem;
        }
        
        .assessment-card h4 i {
            background: rgba(255, 255, 255, 0.1);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .strength h4 i {
            color: var(--primary-purple);
        }
        
        .improvement h4 i {
            color: var(--accent-pink);
        }
        
        .plan h4 i {
            color: #9370DB;
        }
        
        .assessment-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .assessment-card li {
            padding: 12px 0;
            color: #ddd;
            position: relative;
            padding-right: 25px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }
        
        .assessment-card li:before {
            content: "•";
            color: var(--accent-pink);
            position: absolute;
            right: 0;
            top: 12px;
            font-size: 1.8rem;
        }
        
        /* الخاتمة */
        .conclusion-card {
            background: linear-gradient(145deg, rgba(45, 27, 71, 0.9), rgba(74, 35, 90, 0.9));
            border-radius: 20px;
            padding: 40px;
            margin-top: 40px;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
            position: relative;
            overflow: hidden;
        }
        
        .conclusion-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary-purple), var(--accent-pink));
        }
        
        .conclusion-card h3 {
            color: #fff;
            margin-bottom: 30px;
            font-size: 2rem;
            background: linear-gradient(to right, #fff, var(--primary-purple));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 700;
        }
        
        .conclusion-card p {
            color: #ddd;
            line-height: 1.9;
            margin-bottom: 20px;
            max-width: 900px;
            margin-right: auto;
            margin-left: auto;
            font-size: 1.1rem;
        }
        
        /* تذييل الصفحة */
        .footer {
            text-align: center;
            padding: 25px;
            margin-top: 30px;
            color: var(--light-gray);
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 0.9rem;
            background: rgba(45, 27, 71, 0.8);
            border-radius: 15px;
            margin-bottom: 20px;
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        
        /* تصميم متجاوب */
        @media (max-width: 1200px) {
            .nav-icon {
                min-width: 90px;
                padding: 10px 18px;
            }
            
            .logo-title {
                font-size: 1.6rem;
            }
        }
        
        @media (max-width: 992px) {
            .navbar {
                height: 120px;
            }
            
            .nav-container {
                flex-direction: column;
                gap: 15px;
                padding: 15px 20px;
            }
            
            .logo {
                width: 100%;
                justify-content: center;
            }
            
            .nav-icons-container {
                width: 100%;
            }
            
            .nav-icons {
                justify-content: flex-start;
            }
            
            .logo-title {
                font-size: 1.5rem;
            }
            
            .main-content {
                padding: 30px;
            }
            
            .section-title {
                font-size: 1.9rem;
            }
        }
        
        @media (max-width: 768px) {
            .navbar {
                height: auto;
                padding: 15px 0;
            }
            
            .about-header {
                flex-direction: column;
                text-align: center;
            }
            
            .about-info {
                text-align: center;
            }
            
            .avatar {
                width: 120px;
                height: 120px;
                font-size: 3rem;
            }
            
            .about-info h3 {
                font-size: 1.7rem;
            }
            
            .section-title {
                font-size: 1.7rem;
            }
            
            .main-content {
                padding: 25px;
            }
            
            .intro-card, .plan-card, .tech-card, .assessment-card {
                padding: 25px;
            }
            
            .about-card {
                padding: 30px;
            }
        }
        
        @media (max-width: 576px) {
            .nav-icon {
                min-width: 80px;
                padding: 8px 12px;
                height: 50px;
            }
            
            .nav-icon i {
                font-size: 1rem;
            }
            
            .nav-icon span {
                font-size: 0.7rem;
            }
            
            .container {
                padding: 10px;
            }
            
            .main-content {
                padding: 20px;
            }
            
            .logo-title {
                font-size: 1.3rem;
            }
            
            .logo-subtitle {
                font-size: 0.9rem;
            }
            
            .section-title {
                font-size: 1.5rem;
            }
            
            .about-card, .intro-card, .plan-card, .tech-card, .assessment-card {
                padding: 20px;
            }
        }
        
        /* تأثيرات إضافية */
        .fade-in-element {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease, transform 0.8s ease;
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
        
        /* تأثيرات النصوص المتألقة */
        .glow-text {
            text-shadow: 0 0 10px rgba(138, 43, 226, 0.7), 0 0 20px rgba(138, 43, 226, 0.5);
        }
        
        .floating {
            animation: floating 3s ease-in-out infinite;
        }
        
        @keyframes floating {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body>
    <!-- الهيدر الموسع  -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <div class="logo-icon pulse">
                    <i class="fas fa-chalkboard-teacher"></i>
                </div>
                <div class="logo-text">
                    <div class="logo-title glow-text">ملف الإنجاز المهني </div>
                    <div class="logo-subtitle">للمعلمة المتميزة: سارة خويتم الخالدي</div>
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
                        <span>السيرة المهنية</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="planning">
                        <i class="fas fa-calendar-alt"></i>
                        <span>التخطيط</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="strategies">
                        <i class="fas fa-chalkboard-teacher"></i>
                        <span>استراتيجيات</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="evaluation">
                        <i class="fas fa-clipboard-check"></i>
                        <span>التقويم</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="technology">
                        <i class="fas fa-laptop-code"></i>
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
                        <i class="fas fa-book-open"></i>
                        <span>التعلم الذاتي</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="assessment">
                        <i class="fas fa-chart-line"></i>
                        <span>التقييم الذاتي</span>
                    </a>
                    <a href="#" class="nav-icon" data-target="conclusion">
                        <i class="fas fa-flag-checkered"></i>
                        <span>الخاتمة</span>
                    </a>
                </div>
            </div>
        </div>
    </nav>

    <!-- المحتوى الرئيسي -->
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
                                <p>معلمة متخصصة في تدريس الرياضيات للمرحلة الابتدائية، أمتلك شغفاً كبيراً في تطوير مهارات الطلاب والطالبات واستخدام أساليب تربوية حديثة تعتمد على استراتيجيات متنوعة وواضحة لرفع مستوى التحصيل الدراسي.</p>
                            </div>
                        </div>
                        
                        <div class="about-details">
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-heartbeat"></i> فلسفتي التعليمية</h4>
                                <p>أؤمن بأن التعليم هو عملية إبداعية تهدف إلى تنمية التفكير النقدي والإبداعي لدى الطلاب، وليس مجرد نقل للمعرفة. أسعى لجعل الرياضيات مادة محببة وسهلة الفهم من خلال ربطها بالحياة اليومية.</p>
                            </div>
                            
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-rocket"></i> منهجي في التدريس</h4>
                                <p>أعتمد على استراتيجيات تعليمية متنوعة تراعي الفروق الفردية بين الطلاب، مع التركيز على التعلم النشط والتطبيقات العملية التي تجعل الرياضيات حية وملموسة في حياة الطلاب اليومية.</p>
                            </div>
                            
                            <div class="detail-item fade-in-element">
                                <h4><i class="fas fa-trophy"></i> إنجازاتي التربوية</h4>
                                <p>حصلت على تقدير "المعلم المتميز" مرتين، وقمت بتدريب معلمات جديدات على استراتيجيات تدريس الرياضيات الحديثة، وساهمت في رفع معدل نجاح طلابي في اختبارات الرياضيات بنسبة 40%.</p>
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
                        <p>أتطلع إلى إنشاء جيل من الطلاب المتمكنين في الرياضيات، القادرين على تطبيق المفاهيم الرياضية في حياتهم اليومية، والمتمتعين بثقة عالية في قدراتهم العقلية والتحليلية. أسعى لتطوير بيئة تعليمية محفزة تشجع على الإبداع والتفكير النقدي.</p>
                    </div>
                    
                    <div class="intro-card fade-in-element">
                        <h3><i class="fas fa-bullseye"></i> رسالتي التربوية</h3>
                        <p>تقديم تعليم رياضي متميز يلبي احتياجات جميع الطلاب، باستخدام استراتيجيات تدريس مبتكرة وتقنيات تعليمية حديثة. أعمل على تطوير مهارات التفكير الرياضي وحل المشكلات لدى الطلاب، وإعدادهم لمواجهة التحديات الأكاديمية والحياتية.</p>
                    </div>
                    
                    <div class="intro-card fade-in-element">
                        <h3><i class="fas fa-star"></i> قيمي التعليمية</h3>
                        <p>الإبداع، التميز، العدالة، التعاون، والمسؤولية. أؤمن بأهمية تقديم تعليم عالي الجودة لجميع الطلاب بغض النظر عن خلفياتهم وقدراتهم، وأسعى لخلق بيئة تعليمية داعمة تشجع على النمو الشخصي والأكاديمي.</p>
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
                        <p>بكالوريوس تربية - تخصص رياضيات وإحصاء<br>جامعة الطائف - بتقدير امتياز مع مرتبة الشرف</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-book"></i>
                        <h4>التخصص الدقيق</h4>
                        <p>معلمة رياضيات للمرحلة الابتدائية<br>متخصصة في تدريس الرياضيات التطبيقية والتفاعلية</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-briefcase"></i>
                        <h4>المسيرة المهنية</h4>
                        <p>4 سنوات في القطاع الخاص<br>تدريس الرياضيات لطلاب المرحلة الابتدائية في مدارس النخبة الخاصة</p>
                    </div>
                    
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-chalkboard"></i>
                        <h4>المهارات التخصصية</h4>
                        <p>تصميم مناهج رياضية تفاعلية<br>استخدام تقنيات التعليم الحديثة<br>تقييم وتطوير الأداء التعليمي</p>
                    </div>
                </div>
            </section>
            
            <!-- التخطيط للتدريس -->
            <section id="planning" class="section">
                <h2 class="section-title">التخطيط للتدريس</h2>
                <div class="planning-grid">
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-file-alt"></i> نموذج تحضير درس متكامل</h4>
                        <ul>
                            <li>تحليل المحتوى الدراسي وتحديد الأهداف التعليمية</li>
                            <li>تصميم أنشطة تعليمية تفاعلية متنوعة</li>
                            <li>إعداد وسائل تعليمية مبتكرة وجذابة</li>
                            <li>تخطيط أساليب تقييم متنوعة وشاملة</li>
                            <li>إعداد مواد إثرائية وداعمة للتعلم</li>
                        </ul>
                    </div>
                    
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-calendar"></i> توزيع المنهج الدراسي</h4>
                        <ul>
                            <li>توزيع المقرر على الأسابيع الدراسية بشكل متوازن</li>
                            <li>مراعاة المناسبات والأحداث المدرسية والوطنية</li>
                            <li>تخصيص أوقات للمراجعة والتقييم المستمر</li>
                            <li>التنسيق مع فريق العمل لتحقيق التكامل التعليمي</li>
                            <li>مراعاة الفروق الفردية في التخطيط</li>
                        </ul>
                    </div>
                    
                    <div class="plan-card fade-in-element">
                        <h4><i class="fas fa-tasks"></i> خطة تطوير الأداء</h4>
                        <ul>
                            <li>تحديد أهداف تطويرية لكل فصل دراسي</li>
                            <li>تخطيط برامج تدريبية وتطويرية مستمرة</li>
                            <li>تصميم أنشطة تعاونية مع الزملاء</li>
                            <li>متابعة وتقييم التطور المهني المستمر</li>
                            <li>توثيق التجارب الناجحة ونشرها</li>
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
                        <p>استخدام استراتيجيات مثل العصف الذهني، التعلم بالمشاريع، والتعلم القائم على حل المشكلات. أطبق أنشطة عملية مثل تصميم مجسمات هندسية، وتنفيذ مشاريع رياضية صغيرة، وتنظيم مسابقات حسابية تفاعلية.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-users"></i> التعلم التعاوني المنظم</h4>
                        <p>تنظيم الطلاب في مجموعات تعاونية متنوعة المهام. كل مجموعة تتعاون في حل التمارين الرياضية، وتنفيذ المشروعات المشتركة، وتقديم العروض التقديمية التي تعزز مهارات التواصل والعمل الجماعي.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-gamepad"></i> التعليم الترفيهي</h4>
                        <p>دمج الألعاب التعليمية في العملية التعليمية مثل "سودوكو الأطفال"، "بازل الكسور"، و"لعبة الضرب السريع". هذه الألعاب تساعد في تبسيط المفاهيم الرياضية وجعل التعلم تجربة ممتعة ومشوقة.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-lightbulb"></i> التعلم السياقي</h4>
                        <p>ربط الدروس الرياضية بحياة الطلاب اليومية من خلال أمثلة واقعية. في درس الكسور، نستخدم قطع الفاكهة والشوكولاتة، وفي درس القياس نطبق قياسات حقيقية للفصل والملعب المدرسي.</p>
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
                            <li>التقويم التشخيصي القبلي لتحديد مستوى الطلاب</li>
                            <li>التقويم التكويني المستمر خلال العملية التعليمية</li>
                            <li>التقويم الختامي النهائي في نهاية كل وحدة دراسية</li>
                            <li>التقويم الذاتي للطلاب لتطوير مهارات التفكير الناقد</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>تنويع أدوات التقويم</h4>
                        <ul>
                            <li>اختبارات تحريرية متنوعة المستويات</li>
                            <li>مشاريع عملية وتطبيقية</li>
                            <li>ملاحظات أداء أثناء الأنشطة الصفية</li>
                            <li>ملفات إنجاز الطلاب (Portfolios)</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>معالجة الضعف الدراسي</h4>
                        <ul>
                            <li>تحليل نتائج التقويم لتشخيص مواطن الضعف</li>
                            <li>تصميم برامج علاجية فردية وجماعية</li>
                            <li>تنفيذ جلسات تقوية مرنة ومتنوعة</li>
                            <li>متابعة التقدم الأكاديمي بشكل منتظم</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>الاختبارات الإبداعية</h4>
                        <ul>
                            <li>اختبارات تعتمد على حل المشكلات الواقعية</li>
                            <li>اختبارات المشروعات العملية</li>
                            <li>اختبارات الأداء التطبيقي</li>
                            <li>اختبارات التفكير الإبداعي والتحليلي</li>
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
                            <li>منصة مدرستي للتعليم المدمج والتفاعلي</li>
                            <li>برامج الرياضيات التفاعلية مثل Mathletics</li>
                            <li>تطبيقات الواقع المعزز لتعليم الهندسة</li>
                            <li>منصات الألعاب التعليمية مثل Prodigy Math</li>
                            <li>برامج التخطيط الذكي للدروس</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>الاختبارات والتقييم الإلكتروني</h4>
                        <ul>
                            <li>تصميم اختبارات تفاعلية على منصات متخصصة</li>
                            <li>استخدام تقنيات التصحيح الآلي والتحليل</li>
                            <li>إنشاء بنك أسئلة إلكتروني متطور</li>
                            <li>تصميم أنشطة تقييم ذاتي للطلاب</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>مزايا التكامل التقني</h4>
                        <ul>
                            <li>توفير تجارب تعلم شخصية ومتكيفة</li>
                            <li>زيادة تفاعل الطلاب وتحفيزهم للتعلم</li>
                            <li>تمكين التعلم في أي وقت ومن أي مكان</li>
                            <li>تحسين كفاءة عملية التقييم والتغذية الراجعة</li>
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
                        <p>تهدف إلى ربط الرياضيات بالحياة اليومية للطلاب من خلال أنشطة عملية مثل: تصميم ميزانية مصغرة، حساب تكاليف الرحلات، وتحليل البيانات البسيطة من البيئة المحيطة.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-medal"></i> مسابقة "عباقرة الرياضيات"</h4>
                        <p>مسابقة فصلية تشمل تحديات رياضية متنوعة، تهدف إلى تنمية روح المنافسة الإيجابية، واكتشاف المواهب الرياضية، وتشجيع التفكير الإبداعي في حل المسائل.</p>
                    </div>
                    
                    <div class="strategy-card fade-in-element">
                        <h4><i class="fas fa-hands-helping"></i> نادي "أصدقاء الرياضيات"</h4>
                        <p>نادي طلابي تطوعي يهدف إلى تعزيز حب الرياضيات، حيث يشارك الطلاب المتفوقون في مساعدة زملائهم، وتنظيم أنشطة رياضية ممتعة، وتقديم عروض شيقة عن الرياضيات.</p>
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
                            <li>برامج علاجية فردية للطلاب المتعثرين</li>
                            <li>جلسات تقوية مرنة وفق احتياجات كل طالب</li>
                            <li>توفير مواد تعليمية مساندة ومتنوعة</li>
                            <li>شراكات تعليمية مع أولياء الأمور</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>رعاية المتفوقين والمبدعين</h4>
                        <ul>
                            <li>برامج إثرائية متقدمة للمتفوقين</li>
                            <li>مشاركة في مسابقات رياضية محلية</li>
                            <li>توفير فرص قيادية داخل الصف</li>
                            <li>تشجيع البحث العلمي المبكر</li>
                        </ul>
                    </div>
                    
                    <div class="tech-card fade-in-element">
                        <h4>مراعاة التنوع والتعلم الشامل</h4>
                        <ul>
                            <li>تصميم أنشطة تعليمية متنوعة المستويات</li>
                            <li>توفير بدائل تعليمية تلبي جميع الاحتياجات</li>
                            <li>استخدام استراتيجيات تدريس مرنة</li>
                            <li>بناء بيئة صفية داعمة للجميع</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- التعلم الذاتي -->
            <section id="self-learning" class="section">
                <h2 class="section-title">التعلم الذاتي والتطوير المهني</h2>
                <div class="self-learning">
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-book"></i> برنامج القراءة التخصصية</h4>
                        <p>متابعة أحدث الأبحاث والدراسات في مجال تدريس الرياضيات، قراءة الكتب المتخصصة في استراتيجيات التدريس الحديثة، والاطلاع على المجلات التربوية المحلية والعالمية.</p>
                    </div>
                    
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-video"></i> التدريب الإلكتروني المستمر</h4>
                        <p>الالتحاق بالدورات التدريبية عبر الإنترنت، حضور المؤتمرات الافتراضية المتخصصة، متابعة القنوات التعليمية العالمية، والمشاركة في ورش العمل التفاعلية.</p>
                    </div>
                    
                    <div class="learning-card fade-in-element">
                        <h4><i class="fas fa-graduation-cap"></i> الشهادات والاعتمادات</h4>
                        <p>الحصول على شهادات في استخدام التقنية في التعليم، شهادات في استراتيجيات التعلم النشط، اعتماد مدرب معتمد في استراتيجيات تدريس الرياضيات، والمشاركة في برامج التطوير المهني.</p>
                    </div>
                </div>
            </section>
            
            <!-- التقييم الذاتي -->
            <section id="assessment" class="section">
                <h2 class="section-title">التقييم الذاتي والتطوير المهني</h2>
                <div class="assessment-container">
                    <div class="assessment-card strength fade-in-element">
                        <h4><i class="fas fa-check-circle"></i> نقاط القوة والتأثير</h4>
                        <ul>
                            <li>القدرة على تحويل المفاهيم الرياضية المعقدة إلى أنشطة عملية مبسطة</li>
                            <li>تميز في استخدام التقنيات التعليمية الحديثة بشكل إبداعي</li>
                            <li>بناء علاقات إيجابية وفعالة مع الطلاب وأولياء الأمور</li>
                            <li>التخطيط الاستراتيجي للدروس والأنشطة التعليمية</li>
                            <li>المرونة والتكيف مع المتغيرات التعليمية المختلفة</li>
                        </ul>
                    </div>
                    
                    <div class="assessment-card improvement fade-in-element">
                        <h4><i class="fas fa-tools"></i> مجالات التطوير والتحسين</h4>
                        <ul>
                            <li>تطوير مهارات البحث العلمي التربوي المتقدم</li>
                            <li>التعمق في استخدام تحليلات البيانات التعليمية</li>
                            <li>توسيع نطاق تطبيق التعلم القائم على المشاريع</li>
                            <li>الانخراط في مجتمعات التعلم المهنية العالمية</li>
                        </ul>
                    </div>
                    
                    <div class="assessment-card plan fade-in-element">
                        <h4><i class="fas fa-calendar-check"></i> خطة التطوير المستقبلية</h4>
                        <ul>
                            <li>الحصول على ماجستير في مناهج وطرق تدريس الرياضيات</li>
                            <li>تطوير منصة تعليمية تفاعلية متخصصة في الرياضيات</li>
                            <li>إعداد دليل عملي لاستراتيجيات تدريس الرياضيات الحديثة</li>
                            <li>القيام بزيارات تبادلية للمدارس المتميزة عالمياً</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- الخاتمة -->
            <section id="conclusion" class="section">
                <h2 class="section-title">الخاتمة والتطلعات المستقبلية</h2>
                <div class="conclusion-card">
                    <h3>رحلة الإبداع التربوي المستمرة</h3>
                    <p>تمثل مسيرتي التعليمية رحلة متواصلة من التعلم والتطوير، حيث أسعى دائماً إلى تجويد ممارساتي التعليمية والارتقاء بمستوى أدائي المهني. أؤمن بأن المعلم الفعال هو الذي لا يتوقف عن التعلم، بل يظل طالباً للمعارف الجديدة والمهارات المتطورة.</p>
                    <p>أتطلع إلى المساهمة الفعالة في تطوير التعليم الرياضي على مستوى المدرسة والمجتمع المحلي، من خلال تبني المبادرات التربوية المبتكرة، وتدريب الزملاء المعلمين، والمشاركة في وضع السياسات التعليمية التي تخدم مصلحة الطلاب وتطور العملية التعليمية.</p>
                    <p>أهدف إلى ترسيخ ثقافة التميز والإبداع في تدريس الرياضيات، وجعلها مادة محببة ومفهومة لجميع الطلاب، والإسهام في إعداد جيل قادر على مواجهة التحديات المستقبلية بمهارات رياضية متطورة وعقلية تحليلية متميزة.</p>
                    <div style="margin-top: 30px; padding-top: 25px; border-top: 2px solid rgba(138, 43, 226, 0.3);">
                        <p style="font-weight: 700; color: #fff; font-size: 1.2rem;">
                            المعلمة المتميزة<br>
                            <span style="color: var(--accent-pink); font-size: 1.4rem;">سارة خويتم عبدالجبار الخالدي</span><br>
                            معلمة رياضيات - المرحلة الابتدائية<br>
                            ديسمبر 2023
                        </p>
                    </div>
                </div>
            </section>
        </div>
        
        <div class="footer">
            <p>© 2023 ملف الإنجاز  - المعلمة سارة خويتم الخالدي</p>
            <p>جميع الحقوق محفوظة | تم التحديث في ديسمبر 2023 | إصدار 2.0</p>
            <div style="margin-top: 15px;">
                <i class="fas fa-envelope" style="margin: 0 10px; color: var(--accent-pink);"></i>
                <i class="fas fa-phone" style="margin: 0 10px; color: var(--accent-pink);"></i>
                <i class="fas fa-globe" style="margin: 0 10px; color: var(--accent-pink);"></i>
            </div>
        </div>
    </div>

    <script>
        // التحكم في عرض الأقسام
        document.addEventListener('DOMContentLoaded', function() {
            const navIcons = document.querySelectorAll('.nav-icon');
            const sections = document.querySelectorAll('.section');
            
            // تهيئة التأثيرات الحركية
            const fadeElements = document.querySelectorAll('.fade-in-element');
            
            // وظيفة لتحميل الأقسام
            navIcons.forEach(icon => {
                icon.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    // إزالة النشاط من جميع الأيقونات
                    navIcons.forEach(item => {
                        item.classList.remove('active');
                        item.style.transform = 'translateY(0) scale(1)';
                    });
                    
                    // إضافة النشاط للأيقونة المختارة مع تأثير
                    this.classList.add('active');
                    this.style.transform = 'translateY(-4px) scale(1.05)';
                    
                    // إخفاء جميع الأقسام
                    sections.forEach(section => section.classList.remove('active'));
                    
                    // عرض القسم المطلوب
                    const targetId = this.getAttribute('data-target');
                    const targetSection = document.getElementById(targetId);
                    targetSection.classList.add('active');
                    
                    // تفعيل تأثيرات الظهور للعناصر الجديدة
                    setTimeout(() => {
                        const currentFadeElements = targetSection.querySelectorAll('.fade-in-element');
                        currentFadeElements.forEach((el, index) => {
                            setTimeout(() => {
                                el.classList.add('visible');
                                el.style.transitionDelay = `${index * 0.1}s`;
                            }, 100);
                        });
                    }, 200);
                    
                    // إضافة تأثير scroll سلس
                    window.scrollTo({
                        top: document.querySelector('.main-content').offsetTop - 20,
                        behavior: 'smooth'
                    });
                });
            });
            
            // تفعيل تأثيرات الظهور للعناصر عند التمرير
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, observerOptions);
            
            fadeElements.forEach(element => {
                observer.observe(element);
            });
            
            // تفعيل العناصر في الصفحة الأولى عند التحميل
            setTimeout(() => {
                document.querySelectorAll('#about .fade-in-element').forEach((el, index) => {
                    setTimeout(() => {
                        el.classList.add('visible');
                        el.style.transitionDelay = `${index * 0.2}s`;
                    }, 300);
                });
            }, 500);
            
            // تأثيرات عند تحميل الصفحة
            setTimeout(() => {
                document.querySelector('.logo-icon').style.transform = 'rotate(360deg)';
                document.querySelector('.logo-icon').style.transition = 'transform 1s ease';
                
                // تأثيرات إضافية للشعار
                setTimeout(() => {
                    document.querySelector('.logo-title').classList.add('glow-text');
                }, 1000);
            }, 300);
            
            // تحسين العرض على الجوال
            if (window.innerWidth <= 768) {
                document.querySelector('.nav-icons').addEventListener('wheel', function(e) {
                    e.preventDefault();
                    this.scrollLeft += e.deltaY;
                });
            }
            
            // تأثيرات تفاعلية للأيقونات
            navIcons.forEach(icon => {
                icon.addEventListener('mouseenter', function() {
                    if (!this.classList.contains('active')) {
                        this.style.transform = 'translateY(-4px) scale(1.05)';
                        this.style.boxShadow = '0 10px 25px rgba(138, 43, 226, 0.3)';
                    }
                });
                
                icon.addEventListener('mouseleave', function() {
                    if (!this.classList.contains('active')) {
                        this.style.transform = 'translateY(0) scale(1)';
                        this.style.boxShadow = 'none';
                    }
                });
            });
        });
        
        // تأثيرات إضافية عند التمرير
        window.addEventListener('scroll', function() {
            const navbar = document.querySelector('.navbar');
            const scrollY = window.scrollY;
            
            if (scrollY > 50) {
                navbar.style.boxShadow = '0 8px 32px rgba(0, 0, 0, 0.7)';
                navbar.style.backdropFilter = 'blur(15px)';
            } else {
                navbar.style.boxShadow = '0 8px 32px rgba(0, 0, 0, 0.5)';
                navbar.style.backdropFilter = 'blur(10px)';
            }
            
            // تأثيرات على الشعار عند التمرير
            const logoTitle = document.querySelector('.logo-title');
            if (scrollY > 100) {
                logoTitle.style.fontSize = '1.6rem';
                logoTitle.style.transition = 'font-size 0.3s ease';
            } else {
                logoTitle.style.fontSize = '1.8rem';
            }
        });
        
        // تأثيرات إضافية للصفحة
        window.addEventListener('load', function() {
            // إضافة تأثيرات عشوائية للبطاقات
            setTimeout(() => {
                const cards = document.querySelectorAll('.detail-item, .bio-card, .strategy-card');
                cards.forEach((card, index) => {
                    setTimeout(() => {
                        card.style.opacity = '1';
                        card.style.transform = 'translateY(0)';
                    }, index * 100);
                });
            }, 800);
            
            // تأثيرات خفية للخلفية
            const backgroundEffect = document.createElement('div');
            backgroundEffect.style.position = 'fixed';
            backgroundEffect.style.top = '0';
            backgroundEffect.style.left = '0';
            backgroundEffect.style.width = '100%';
            backgroundEffect.style.height = '100%';
            backgroundEffect.style.background = 'radial-gradient(circle at 50% 50%, rgba(138, 43, 226, 0.1) 0%, transparent 50%)';
            backgroundEffect.style.pointerEvents = 'none';
            backgroundEffect.style.zIndex = '-1';
            document.body.appendChild(backgroundEffect);
        });
    </script>
</body>
</html>
