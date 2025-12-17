
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
            /* ألوان خردلية وأنيقة مع نصوص بنفسجية */
            --primary-color: #AC8A3C; /* اللون الخردلي الأساسي */
            --secondary-color: #431b6f; /* بنفسجي للعناوين */
            --accent-color: #5D2A9A; /* بنفسجي فاتح */
            --background-color: #F8F5E6; /* بيج فاتح جداً */
            --card-bg: #FFFFFF;
            --light-gray: #F9F7F0; /* بيج فاتح */
            --text-color: #431b6f; /* بنفسجي للنصوص */
            --text-light: #6B4F8C; /* بنفسجي فاتح للنصوص الثانوية */
            --border-color: #E8E4D5;
            --gradient-primary: linear-gradient(135deg, #AC8A3C 0%, #8B6F2A 100%);
            --gradient-light: linear-gradient(135deg, #F9F7F0 0%, #E8E4D5 100%);
            --gradient-purple: linear-gradient(135deg, #431b6f 0%, #5D2A9A 100%); /* تدرج بنفسجي */
        }
        
        body {
            background: var(--background-color);
            color: var(--text-color);
            line-height: 1.7;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
            -webkit-text-size-adjust: 100%;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 20px;
            width: 100%;
        }
        
        /* الهيدر المصغر للجوال */
        .navbar {
            background: linear-gradient(135deg, #431b6f 0%, #5D2A9A 100%); /* تدرج بنفسجي */
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(67, 27, 111, 0.2);
            height: auto;
            min-height: 70px;
            border-bottom: none;
            padding: 0;
        }
        
        .nav-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 15px;
            gap: 15px;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-weight: 600;
            font-size: 1rem;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
            width: 100%;
            justify-content: center;
            text-align: center;
        }
        
        .logo-icon {
            background: var(--gradient-purple);
            width: 50px;
            height: 50px;
            min-width: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 6px 20px rgba(67, 27, 111, 0.3);
            border: 2px solid rgba(255, 255, 255, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .logo-icon i {
            font-size: 1.4rem;
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
            color: white;
            font-weight: 700;
            line-height: 1.3;
            letter-spacing: -0.3px;
        }
        
        .logo-subtitle {
            font-size: 0.85rem;
            color: rgba(255, 255, 255, 0.9);
            margin-top: 4px;
            font-weight: 400;
        }
        
        /* شريط الأيقونات المصغر */
        .nav-icons-container {
            background: rgba(255, 255, 255, 0.15);
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
            padding: 3px;
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
            padding: 8px 10px;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            text-decoration: none;
            color: white;
            border-radius: 12px;
            min-width: 65px;
            height: 45px;
            position: relative;
            overflow: hidden;
            background: rgba(255, 255, 255, 0.1);
            flex-shrink: 0;
            touch-action: manipulation;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .nav-icon:hover, .nav-icon.active {
            background: rgba(255, 255, 255, 0.25);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(255, 255, 255, 0.2);
        }
        
        .nav-icon.active {
            background: rgba(255, 255, 255, 0.3);
            box-shadow: 0 4px 15px rgba(255, 255, 255, 0.25);
        }
        
        .nav-icon i {
            font-size: 1rem;
            margin-bottom: 3px;
            z-index: 1;
        }
        
        .nav-icon span {
            font-size: 0.65rem;
            font-weight: 500;
            white-space: nowrap;
            z-index: 1;
        }
        
        /* المحتوى الرئيسي المعدّل للجوال */
        .main-content {
            background: var(--card-bg);
            border-radius: 25px;
            box-shadow: 
                0 15px 35px rgba(67, 27, 111, 0.08),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            margin-top: 20px;
            margin-bottom: 30px;
            padding: 30px 25px;
            min-height: auto;
            border: 1px solid rgba(232, 228, 213, 0.8);
            position: relative;
            overflow: hidden;
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
            color: var(--secondary-color);
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px solid rgba(67, 27, 111, 0.1);
            position: relative;
            font-size: 1.8rem;
            font-weight: 800;
            line-height: 1.3;
            letter-spacing: -0.5px;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -2px;
            right: 0;
            width: 100px;
            height: 4px;
            background: var(--gradient-purple);
            border-radius: 2px;
        }
        
        /* قسم نبذة عني للجوال */
        .about-section {
            max-width: 100%;
            margin: 0 auto;
        }
        
        .about-card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 30px 25px;
            margin-bottom: 30px;
            border-left: none;
            box-shadow: 
                0 15px 30px rgba(67, 27, 111, 0.05),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            animation: fadeIn 0.5s ease;
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(232, 228, 213, 0.8);
        }
        
        .about-header {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 30px;
            gap: 25px;
            position: relative;
            z-index: 1;
            text-align: center;
        }
        
        .avatar {
            width: 140px;
            height: 140px;
            border-radius: 50%;
            background: var(--gradient-purple);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3.5rem;
            box-shadow: 
                0 10px 30px rgba(67, 27, 111, 0.2),
                inset 0 3px 6px rgba(255, 255, 255, 0.3);
            border: 4px solid rgba(255, 255, 255, 0.5);
        }
        
        .about-info h3 {
            color: var(--secondary-color);
            margin-bottom: 15px;
            font-size: 1.8rem;
            font-weight: 800;
            line-height: 1.3;
            letter-spacing: -0.5px;
        }
        
        .about-info p {
            color: var(--text-color);
            line-height: 1.7;
            margin-bottom: 12px;
            font-size: 1.05rem;
        }
        
        .highlight {
            color: var(--secondary-color);
            font-weight: 700;
        }
        
        .about-details {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .detail-item {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border-top: none;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .detail-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .detail-item h4 {
            color: var(--secondary-color);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.3rem;
            font-weight: 700;
        }
        
        .detail-item h4 i {
            color: white;
            background: var(--gradient-purple);
            width: 40px;
            height: 40px;
            min-width: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.3);
        }
        
        .detail-item p {
            color: var(--text-color);
            line-height: 1.7;
            font-size: 1.05rem;
        }
        
        /* قسم الشواهد الوظيفية */
        .certificates-section {
            max-width: 100%;
            margin: 0 auto;
        }
        
        .certificates-card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 50px 30px;
            margin-bottom: 30px;
            text-align: center;
            border: 2px dashed rgba(67, 27, 111, 0.3);
            box-shadow: 
                0 15px 30px rgba(67, 27, 111, 0.05),
                inset 0 1px 0 rgba(255, 255, 255, 0.8);
            animation: fadeIn 0.5s ease;
            position: relative;
            overflow: hidden;
        }
        
        .certificates-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 35px;
        }
        
        .hourglass-container {
            position: relative;
            width: 140px;
            height: 140px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .hourglass {
            font-size: 4.5rem;
            color: var(--secondary-color);
            animation: hourglassRotate 3s infinite ease-in-out;
        }
        
        @keyframes hourglassRotate {
            0% { transform: rotate(0deg); }
            25% { transform: rotate(90deg); }
            50% { transform: rotate(180deg); }
            75% { transform: rotate(270deg); }
            100% { transform: rotate(360deg); }
        }
        
        .hourglass-shadow {
            position: absolute;
            bottom: -10px;
            width: 100px;
            height: 20px;
            background: rgba(67, 27, 111, 0.1);
            border-radius: 50%;
            filter: blur(8px);
            animation: shadowPulse 3s infinite ease-in-out;
        }
        
        @keyframes shadowPulse {
            0%, 100% { width: 100px; opacity: 0.1; }
            50% { width: 110px; opacity: 0.2; }
        }
        
        .certificates-text {
            text-align: center;
        }
        
        .certificates-text h3 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            font-size: 2rem;
            font-weight: 800;
        }
        
        .certificates-text p {
            color: var(--secondary-color);
            font-size: 1.4rem;
            font-weight: 700;
            line-height: 1.5;
            background: var(--light-gray);
            padding: 20px 25px;
            border-radius: 15px;
            border: 1px solid rgba(232, 228, 213, 0.8);
        }
        
        /* المقدمة - للجوال */
        .intro-section {
            max-width: 100%;
            margin: 0 auto;
        }
        
        .intro-card {
            background: var(--card-bg);
            border-radius: 18px;
            padding: 25px;
            margin-bottom: 25px;
            border-right: none;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .intro-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .intro-card h3 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }
        
        .intro-card h3 i {
            color: white;
            background: var(--gradient-purple);
            width: 45px;
            height: 45px;
            min-width: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.3);
            margin-top: 2px;
        }
        
        .intro-card p {
            color: var(--text-color);
            line-height: 1.7;
            margin-bottom: 15px;
            font-size: 1.05rem;
        }
        
        /* السيرة المهنية المختصرة للجوال */
        .bio-grid {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .bio-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border: 1px solid rgba(232, 228, 213, 0.8);
            text-align: center;
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .bio-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .bio-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient-purple);
        }
        
        .bio-card i {
            font-size: 2.8rem;
            color: var(--secondary-color);
            margin-bottom: 20px;
            background: rgba(249, 247, 240, 0.8);
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-left: auto;
            margin-right: auto;
            border: 2px solid rgba(232, 228, 213, 0.8);
        }
        
        .bio-card h4 {
            color: var(--secondary-color);
            margin-bottom: 15px;
            font-size: 1.4rem;
            font-weight: 700;
        }
        
        .bio-card p {
            color: var(--text-color);
            font-size: 1.05rem;
            line-height: 1.7;
        }
        
        /* التخطيط للتدريس للجوال */
        .planning-grid {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .plan-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border-top: none;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .plan-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .plan-card h4 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }
        
        .plan-card h4 i {
            color: white;
            background: var(--gradient-purple);
            width: 45px;
            height: 45px;
            min-width: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.3);
            margin-top: 2px;
        }
        
        .plan-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .plan-card li {
            padding: 12px 0;
            border-bottom: 1px solid rgba(232, 228, 213, 0.8);
            position: relative;
            padding-right: 30px;
            color: var(--text-color);
            font-size: 1.05rem;
            line-height: 1.6;
        }
        
        .plan-card li:before {
            content: "•";
            color: var(--secondary-color);
            font-size: 1.8rem;
            position: absolute;
            right: 0;
            top: 10px;
        }
        
        /* استراتيجيات التدريس للجوال */
        .strategy-container {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .strategy-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border: 1px solid rgba(232, 228, 213, 0.8);
            position: relative;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .strategy-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .strategy-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 100%;
            background: var(--gradient-purple);
        }
        
        .strategy-card h4 {
            color: var(--secondary-color);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }
        
        .strategy-card h4 i {
            color: white;
            background: var(--gradient-purple);
            width: 45px;
            height: 45px;
            min-width: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.3);
            margin-top: 2px;
        }
        
        .strategy-card p {
            color: var(--text-color);
            font-size: 1.05rem;
            line-height: 1.7;
        }
        
        /* التقنية والمبادرات للجوال */
        .tech-grid {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .tech-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border-left: none;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .tech-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .tech-card h4 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            font-size: 1.4rem;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(67, 27, 111, 0.2);
            font-weight: 700;
        }
        
        .tech-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .tech-card li {
            padding: 12px 0;
            color: var(--text-color);
            position: relative;
            padding-right: 30px;
            border-bottom: 1px solid rgba(232, 228, 213, 0.8);
            font-size: 1.05rem;
            line-height: 1.6;
        }
        
        .tech-card li:before {
            content: "✓";
            color: var(--secondary-color);
            position: absolute;
            right: 0;
            top: 12px;
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        /* التعلم الذاتي للجوال */
        .self-learning {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .learning-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .learning-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .learning-card h4 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }
        
        .learning-card h4 i {
            color: white;
            background: var(--gradient-purple);
            width: 45px;
            height: 45px;
            min-width: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.3);
            margin-top: 2px;
        }
        
        .learning-card p {
            color: var(--text-color);
            line-height: 1.7;
            font-size: 1.05rem;
        }
        
        /* التقييم الذاتي للجوال */
        .assessment-container {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 30px;
        }
        
        .assessment-card {
            background: var(--light-gray);
            border-radius: 18px;
            padding: 25px;
            border-top: none;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
            border: 1px solid rgba(232, 228, 213, 0.8);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .assessment-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.08);
        }
        
        .strength {
            border-top: 4px solid #8A4FBF; /* بنفسجي متوسط */
        }
        
        .improvement {
            border-top: 4px solid #B86CF5; /* بنفسجي فاتح */
        }
        
        .plan {
            border-top: 4px solid #431b6f; /* بنفسجي غامق */
        }
        
        .assessment-card h4 {
            color: var(--secondary-color);
            margin-bottom: 20px;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            font-size: 1.4rem;
            line-height: 1.3;
            font-weight: 700;
        }
        
        .assessment-card h4 i {
            background: rgba(255, 255, 255, 0.9);
            width: 45px;
            height: 45px;
            min-width: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            margin-top: 2px;
            color: var(--secondary-color);
            box-shadow: 0 4px 10px rgba(67, 27, 111, 0.1);
        }
        
        .assessment-card ul {
            list-style-type: none;
            padding-right: 15px;
        }
        
        .assessment-card li {
            padding: 12px 0;
            color: var(--text-color);
            position: relative;
            padding-right: 30px;
            border-bottom: 1px solid rgba(232, 228, 213, 0.8);
            font-size: 1.05rem;
            line-height: 1.6;
        }
        
        .assessment-card li:before {
            content: "•";
            color: var(--secondary-color);
            position: absolute;
            right: 0;
            top: 12px;
            font-size: 1.8rem;
        }
        
        /* الخاتمة للجوال */
        .conclusion-card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 30px 25px;
            margin-top: 35px;
            text-align: center;
            border: 1px solid rgba(232, 228, 213, 0.8);
            box-shadow: 0 15px 30px rgba(67, 27, 111, 0.05);
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
            background: var(--gradient-purple);
        }
        
        .conclusion-card h3 {
            color: var(--secondary-color);
            margin-bottom: 25px;
            font-size: 1.8rem;
            line-height: 1.3;
            font-weight: 800;
        }
        
        .conclusion-card p {
            color: var(--text-color);
            line-height: 1.7;
            margin-bottom: 20px;
            font-size: 1.05rem;
            text-align: right;
        }
        
        /* تذييل الصفحة للجوال */
        .footer {
            text-align: center;
            padding: 25px 20px;
            margin-top: 25px;
            color: var(--text-light);
            border-top: 1px solid rgba(232, 228, 213, 0.8);
            font-size: 0.9rem;
            background: var(--card-bg);
            border-radius: 15px;
            margin-bottom: 20px;
            line-height: 1.6;
            box-shadow: 0 8px 20px rgba(67, 27, 111, 0.03);
        }
        
        /* تحسينات للشاشات المتوسطة والكبيرة */
        @media (min-width: 576px) {
            .container {
                padding: 0 25px;
            }
            
            .nav-icon {
                min-width: 70px;
                padding: 10px 12px;
            }
            
            .nav-icon span {
                font-size: 0.7rem;
            }
            
            .logo-title {
                font-size: 1.6rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .about-header {
                flex-direction: row;
                text-align: right;
                align-items: center;
            }
            
            .avatar {
                width: 160px;
                height: 160px;
                font-size: 4rem;
            }
            
            .about-info h3 {
                font-size: 2rem;
            }
        }
        
        @media (min-width: 768px) {
            .navbar {
                height: 90px;
                padding: 0;
            }
            
            .nav-container {
                flex-direction: row;
                justify-content: space-between;
                padding: 0 30px;
                height: 90px;
                gap: 0;
            }
            
            .logo {
                width: auto;
                justify-content: flex-start;
            }
            
            .nav-icons-container {
                width: auto;
                max-width: 75%;
            }
            
            .logo-title {
                font-size: 1.8rem;
            }
            
            .logo-subtitle {
                font-size: 0.9rem;
            }
            
            .main-content {
                padding: 40px 35px;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
            
            .about-details {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .bio-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .planning-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .strategy-container {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .tech-grid {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .self-learning {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
            
            .assessment-container {
                display: grid;
                grid-template-columns: repeat(2, 1fr);
                gap: 30px;
            }
        }
        
        @media (min-width: 992px) {
            .nav-icons-container {
                max-width: 80%;
            }
            
            .nav-icon {
                min-width: 75px;
                padding: 10px 15px;
            }
            
            .nav-icon span {
                font-size: 0.75rem;
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
                min-width: 80px;
            }
            
            .logo-title {
                font-size: 2rem;
            }
            
            .planning-grid {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .strategy-container {
                grid-template-columns: repeat(4, 1fr);
            }
        }
        
        @media (max-height: 600px) and (orientation: landscape) {
            .navbar {
                height: auto;
                min-height: 60px;
            }
            
            .nav-container {
                flex-direction: row;
                padding: 10px 15px;
            }
            
            .logo-icon {
                width: 40px;
                height: 40px;
                min-width: 40px;
            }
            
            .logo-icon i {
                font-size: 1.1rem;
            }
            
            .logo-title {
                font-size: 1.2rem;
            }
            
            .nav-icon {
                min-width: 60px;
                height: 40px;
                padding: 6px 8px;
            }
            
            .nav-icon i {
                font-size: 0.9rem;
                margin-bottom: 2px;
            }
            
            .nav-icon span {
                font-size: 0.6rem;
            }
        }
        
        .nav-icon:active {
            transform: scale(0.95);
            transition: transform 0.1s ease;
        }
        
        input, select, textarea {
            font-size: 16px;
        }
        
        .fade-in-element {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.5s ease, transform 0.5s ease;
        }
        
        .fade-in-element.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
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
        
        .no-select {
            -webkit-touch-callout: none;
            -webkit-user-select: none;
            -khtml-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
        }
        
        * {
            -webkit-overflow-scrolling: touch;
        }
        
        @supports (-webkit-touch-callout: none) {
            .navbar {
                position: -webkit-sticky;
            }
        }
    </style>
</head>
<body class="no-select">
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">
                <div class="logo-icon pulse">
                    <i class="fas fa-chalkboard-teacher"></i>
                </div>
                <div class="logo-text">
                    <div class="logo-title">ملف الإنجاز المهني</div>
                    <div class="logo-subtitle">المعلمة سارة الخالدي</div>
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
                    <a href="#" class="nav-icon" data-target="certificates">
                        <i class="fas fa-certificate"></i>
                        <span>الشواهد</span>
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

    <div class="container">
        <div class="main-content">
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
                                <p>حصلت على تقدير "المعلم المتميز" في القطاع الخاص، وساهمت في رفع معدل نجاح طلابي في اختبارات الرياضيات بنسبة 40%.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
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
            
            <section id="bio" class="section">
                <h2 class="section-title">السيرة المهنية المختصرة</h2>
                <div class="bio-grid">
                    <div class="bio-card fade-in-element">
                        <i class="fas fa-graduation-cap"></i>
                        <h4>المؤهل العلمي</h4>
                        <p>بكالوريوس - تخصص رياضيات وإحصاء - جامعة الطائف</p>
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
            
            <section id="certificates" class="section">
                <h2 class="section-title">الشواهد الوظيفية</h2>
                <div class="certificates-section">
                    <div class="certificates-card">
                        <div class="certificates-content">
                            <div class="hourglass-container">
                                <div class="hourglass">
                                    <i class="fas fa-hourglass-half"></i>
                                </div>
                                <div class="hourglass-shadow"></div>
                            </div>
                            <div class="certificates-text">
                                <h3>الشواهد والتقديرات الوظيفية</h3>
                                <p>سيتم إضافة جميع الشواهد الوظيفية قريباً</p>
                                <p style="margin-top: 20px; color: var(--secondary-color); font-size: 1rem;">
                                    <i class="fas fa-spinner fa-spin" style="margin-left: 5px;"></i>
                                    جاري تحديث المحتوى
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            
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
            
            <section id="conclusion" class="section">
                <h2 class="section-title">الخاتمة والتطلعات</h2>
                <div class="conclusion-card">
                    <h3>رحلة الإبداع التربوي المستمرة</h3>
                    <p>تمثل مسيرتي التعليمية رحلة متواصلة من التعلم والتطوير، حيث أسعى دائماً إلى تجويد ممارساتي التعليمية والارتقاء بمستوى أدائي المهني.</p>
                    <p>أتطلع إلى المساهمة الفعالة في تطوير التعليم الرياضي على مستوى المدرسة والمجتمع المحلي، من خلال تبني المبادرات التربوية المبتكرة.</p>
                    <p>أهدف إلى ترسيخ ثقافة التميز والإبداع في تدريس الرياضيات، وجعلها مادة محببة ومفهومة لجميع الطلاب.</p>
                    <div style="margin-top: 25px; padding-top: 20px; border-top: 2px solid rgba(232, 228, 213, 0.8);">
                        <p style="font-weight: 700; color: var(--secondary-color); font-size: 1.1rem;">
                            المعلمة<br>
                            <span style="color: var(--secondary-color); font-size: 1.2rem;">سارة خويتم الخالدي</span><br>
                            معلمة رياضيات - المرحلة الابتدائية<br>
                            ديسمبر 2025
                        </p>
                    </div>
                </div>
            </section>
        </div>
        
        <div class="footer">
            <p>© 2025 ملف الإنجاز المهني - المعلمة سارة خويتم الخالدي</p>
            <p>جميع الحقوق محفوظة | تم التحديث في ديسمبر 2025</p>
            <div style="margin-top: 15px;">
                <i class="fas fa-envelope" style="margin: 0 10px; color: var(--secondary-color);"></i>
                <i class="fas fa-phone" style="margin: 0 10px; color: var(--secondary-color);"></i>
                <i class="fas fa-globe" style="margin: 0 10px; color: var(--secondary-color);"></i>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const navIcons = document.querySelectorAll('.nav-icon');
            const sections = document.querySelectorAll('.section');
            
            function loadSection(targetId) {
                navIcons.forEach(item => item.classList.remove('active'));
                
                const targetIcon = document.querySelector(`.nav-icon[data-target="${targetId}"]`);
                if (targetIcon) {
                    targetIcon.classList.add('active');
                }
                
                sections.forEach(section => section.classList.remove('active'));
                
                const targetSection = document.getElementById(targetId);
                if (targetSection) {
                    targetSection.classList.add('active');
                }
                
                setTimeout(() => {
                    const currentFadeElements = targetSection.querySelectorAll('.fade-in-element');
                    currentFadeElements.forEach((el, index) => {
                        setTimeout(() => {
                            el.classList.add('visible');
                        }, index * 50);
                    });
                }, 100);
                
                if (window.innerWidth < 768) {
                    window.scrollTo({
                        top: 0,
                        behavior: 'smooth'
                    });
                }
            }
            
            navIcons.forEach(icon => {
                icon.addEventListener('click', function(e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('data-target');
                    loadSection(targetId);
                });
                
                icon.addEventListener('touchstart', function() {
                    this.style.opacity = '0.8';
                });
                
                icon.addEventListener('touchend', function() {
                    this.style.opacity = '1';
                });
            });
            
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
            
            setTimeout(() => {
                document.querySelectorAll('#about .fade-in-element').forEach((el, index) => {
                    setTimeout(() => {
                        el.classList.add('visible');
                    }, index * 150);
                });
            }, 300);
            
            const navIconsContainer = document.querySelector('.nav-icons');
            let isScrolling = false;
            
            if (navIconsContainer) {
                navIconsContainer.addEventListener('touchmove', function(e) {
                    if (!isScrolling) {
                        isScrolling = true;
                        setTimeout(() => {
                            isScrolling = false;
                        }, 100);
                    }
                });
            }
            
            document.body.addEventListener('touchmove', function(e) {
                if (e.target.closest('.nav-icons')) {
                    return;
                }
            }, { passive: true });
            
            let lastScrollTop = 0;
            const navbar = document.querySelector('.navbar');
            
            window.addEventListener('scroll', function() {
                const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
                
                if (scrollTop > lastScrollTop && scrollTop > 100) {
                    navbar.style.transform = 'translateY(-100%)';
                    navbar.style.transition = 'transform 0.3s ease';
                } else {
                    navbar.style.transform = 'translateY(0)';
                }
                
                lastScrollTop = scrollTop;
            });
            
            loadSection('about');
        });
        
        window.addEventListener('load', function() {
            setTimeout(() => {
                document.body.style.opacity = '1';
                document.body.style.transition = 'opacity 0.3s ease';
            }, 100);
            
            if (window.innerWidth <= 480) {
                document.querySelectorAll('p, li, span').forEach(el => {
                    const currentSize = parseFloat(window.getComputedStyle(el).fontSize);
                    if (currentSize > 14) {
                        el.style.fontSize = (currentSize * 0.95) + 'px';
                    }
                });
            }
            
            if (/iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream) {
                document.body.style.webkitBackfaceVisibility = 'hidden';
                document.body.style.webkitTransform = 'translateZ(0)';
            }
        });
        
        document.addEventListener('touchstart', function(event) {
            if (event.target.tagName === 'INPUT' || event.target.tagName === 'TEXTAREA') {
                event.target.style.fontSize = '16px';
            }
        });
    </script>
</body>
</html>
