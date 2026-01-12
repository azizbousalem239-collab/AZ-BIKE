<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Location Motos Électriques - Agadir Tikiouine</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #1a2e1a;
            background: #0a1a0a;
            overflow-x: hidden;
        }
        
        @keyframes gradientFlow {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-30px) rotate(5deg); }
        }
        
        @keyframes glow {
            0%, 100% { 
                box-shadow: 0 0 20px rgba(34,197,94,0.3),
                           0 0 40px rgba(34,197,94,0.2),
                           0 0 60px rgba(34,197,94,0.1);
            }
            50% { 
                box-shadow: 0 0 30px rgba(34,197,94,0.5),
                           0 0 60px rgba(34,197,94,0.3),
                           0 0 90px rgba(34,197,94,0.2);
            }
        }
        
        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-100px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        @keyframes shine {
            0% { left: -150%; }
            100% { left: 150%; }
        }
        
        @keyframes rotateGlow {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.05); opacity: 0.8; }
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(10,26,10,0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 1rem 2rem;
            border-bottom: 2px solid rgba(34,197,94,0.3);
            box-shadow: 0 5px 20px rgba(0,0,0,0.5);
            animation: slideDown 0.5s ease;
        }

        nav .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        nav .logo {
            color: #22c55e;
            font-size: 1.5rem;
            font-weight: bold;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: #e0e0e0;
            text-decoration: none;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 5px;
        }

        nav a:hover {
            color: #22c55e;
            background: rgba(34,197,94,0.1);
            transform: translateY(-2px);
        }
        
        header {
            background: linear-gradient(135deg, #0a1a0a 0%, #1a3e1a 25%, #1b4d1b 50%, #1a3e1a 75%, #0a1a0a 100%);
            background-size: 400% 400%;
            animation: gradientFlow 15s ease infinite;
            color: white;
            text-align: center;
            padding: 10rem 1rem 6rem;
            position: relative;
            overflow: hidden;
            border-bottom: 3px solid #22c55e;
            margin-top: 60px;
        }
        
        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(34,197,94,0.1) 0%, transparent 70%);
            animation: rotateGlow 20s linear infinite;
        }
        
        header::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 50%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            animation: shine 4s infinite;
        }
        
        header h1 {
            font-size: 4rem;
            margin-bottom: 1rem;
            animation: fadeInUp 1s ease;
            text-shadow: 0 0 20px rgba(34,197,94,0.5),
                        0 0 40px rgba(34,197,94,0.3),
                        2px 2px 4px rgba(0,0,0,0.5);
            position: relative;
            z-index: 2;
            background: linear-gradient(45deg, #fff, #22c55e, #fff);
            background-size: 200% 200%;
            animation: gradientFlow 3s ease infinite;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        header p {
            font-size: 1.5rem;
            opacity: 0.95;
            animation: fadeInUp 1s ease 0.3s backwards;
            position: relative;
            z-index: 2;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 3rem;
            margin-top: 3rem;
            position: relative;
            z-index: 2;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
            padding: 1.5rem 2rem;
            background: rgba(34,197,94,0.1);
            border-radius: 15px;
            border: 2px solid rgba(34,197,94,0.3);
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
        }

        .stat-item:hover {
            transform: translateY(-10px);
            background: rgba(34,197,94,0.2);
            border-color: #22c55e;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: bold;
            color: #22c55e;
            text-shadow: 0 0 20px rgba(34,197,94,0.5);
        }

        .stat-label {
            font-size: 1rem;
            color: #e0e0e0;
            margin-top: 0.5rem;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 3rem 1rem;
        }
        
        .section {
            margin-bottom: 5rem;
            animation: fadeInUp 0.8s ease;
            background: linear-gradient(135deg, rgba(26,62,26,0.9) 0%, rgba(27,77,27,0.8) 100%);
            padding: 4rem 2rem;
            border-radius: 30px;
            backdrop-filter: blur(10px);
            box-shadow: 0 20px 60px rgba(0,0,0,0.5),
                       inset 0 0 40px rgba(34,197,94,0.05);
            border: 1px solid rgba(34,197,94,0.2);
        }
        
        .section h2 {
            color: #22c55e;
            margin-bottom: 3rem;
            font-size: 3rem;
            text-align: center;
            position: relative;
            padding-bottom: 1.5rem;
            text-shadow: 0 0 20px rgba(34,197,94,0.5),
                        0 0 40px rgba(34,197,94,0.3);
            animation: fadeInUp 0.8s ease;
        }
        
        .section h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 150px;
            height: 5px;
            background: linear-gradient(90deg, transparent, #22c55e, transparent);
            border-radius: 5px;
            animation: glow 2s ease-in-out infinite;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }
        
        .feature-card {
            background: linear-gradient(135deg, rgba(34,197,94,0.1) 0%, rgba(255,255,255,0.05) 100%);
            padding: 2.5rem;
            border-radius: 20px;
            text-align: center;
            transition: all 0.5s ease;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            position: relative;
            overflow: hidden;
            border: 2px solid rgba(34,197,94,0.3);
            backdrop-filter: blur(10px);
            cursor: pointer;
        }
        
        .feature-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(34,197,94,0.2) 0%, transparent 70%);
            opacity: 0;
            transition: opacity 0.5s;
        }
        
        .feature-card:hover::before {
            opacity: 1;
            animation: rotateGlow 3s linear infinite;
        }
        
        .feature-card:hover {
            transform: translateY(-15px) scale(1.05);
            box-shadow: 0 20px 50px rgba(34,197,94,0.4),
                       0 0 50px rgba(34,197,94,0.2);
            border-color: #22c55e;
        }
        
        .feature-card h3 {
            color: #22c55e;
            margin-bottom: 1rem;
            font-size: 1.8rem;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }
        
        .feature-card p {
            color: #e0e0e0;
            font-size: 1.1rem;
        }
        
        .motos-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 4rem;
            margin-top: 3rem;
        }
        
        .moto-card {
            background: linear-gradient(135deg, rgba(26,62,26,0.95) 0%, rgba(27,77,27,0.9) 100%);
            border-radius: 30px;
            overflow: hidden;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5),
                       0 0 40px rgba(34,197,94,0.2);
            transition: all 0.6s ease;
            position: relative;
            border: 2px solid rgba(34,197,94,0.3);
            animation: float 6s ease-in-out infinite;
        }
        
        .moto-card:nth-child(2) {
            animation-delay: 2s;
        }
        
        .moto-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(34,197,94,0.1) 0%, transparent 100%);
            opacity: 0;
            transition: opacity 0.5s;
            z-index: 1;
        }
        
        .moto-card:hover::before {
            opacity: 1;
        }
        
        .moto-card:hover {
            transform: translateY(-20px) scale(1.03);
            box-shadow: 0 30px 80px rgba(34,197,94,0.5),
                       0 0 60px rgba(34,197,94,0.3);
            border-color: #22c55e;
        }
        
        .moto-card img {
            width: 100%;
            height: 320px;
            object-fit: cover;
            transition: transform 0.6s ease;
            position: relative;
        }
        
        .moto-card:hover img {
            transform: scale(1.15);
        }
        
        .moto-info {
            padding: 2.5rem;
            background: linear-gradient(180deg, rgba(26,62,26,0.9) 0%, rgba(27,77,27,0.8) 100%);
            position: relative;
            z-index: 2;
        }
        
        .moto-info h3 {
            color: #22c55e;
            margin-bottom: 1rem;
            font-size: 1.8rem;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }
        
        .moto-info p {
            color: #e0e0e0;
            font-size: 1.1rem;
        }

        .moto-badge {
            position: absolute;
            top: 20px;
            right: 20px;
            background: linear-gradient(135deg, #22c55e, #16a34a);
            color: #0a1a0a;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-weight: bold;
            z-index: 3;
            animation: pulse 2s ease infinite;
        }
        
        .offers-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }
        
        .offer-card {
            background: linear-gradient(135deg, rgba(34,197,94,0.15) 0%, rgba(255,255,255,0.05) 100%);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 40px rgba(0,0,0,0.4);
            text-align: center;
            transition: all 0.5s ease;
            cursor: pointer;
            border: 2px solid rgba(34,197,94,0.2);
            position: relative;
        }
        
        .offer-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(34,197,94,0.3), transparent);
            transition: left 0.6s;
        }
        
        .offer-card:hover::before {
            left: 100%;
        }
        
        .offer-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 25px 60px rgba(34,197,94,0.4),
                       0 0 40px rgba(34,197,94,0.3);
            border-color: #22c55e;
        }
        
        .offer-card img {
            width: 100%;
            height: 220px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .offer-card:hover img {
            transform: scale(1.2);
        }
        
        .offer-content {
            padding: 2rem;
            background: linear-gradient(180deg, rgba(26,62,26,0.9) 0%, rgba(27,77,27,0.8) 100%);
        }
        
        .offer-content h3 {
            color: #22c55e;
            margin-bottom: 0.8rem;
            font-size: 1.5rem;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }
        
        .offer-content p {
            color: #e0e0e0;
            font-size: 1.05rem;
        }
        
        .contact-info {
            background: linear-gradient(135deg, #1a3e1a 0%, #1b4d1b 50%, #1a3e1a 100%);
            background-size: 200% 200%;
            animation: gradientFlow 10s ease infinite;
            color: white;
            padding: 4rem;
            border-radius: 30px;
            margin-top: 3rem;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5),
                       0 0 60px rgba(34,197,94,0.3),
                       inset 0 0 60px rgba(34,197,94,0.1);
            position: relative;
            overflow: hidden;
            border: 3px solid rgba(34,197,94,0.5);
        }
        
        .contact-info::before {
            content: '⚡';
            position: absolute;
            font-size: 20rem;
            opacity: 0.05;
            right: -80px;
            top: -80px;
            animation: float 8s ease-in-out infinite;
        }
        
        .contact-info::after {
            content: '🏍️';
            position: absolute;
            font-size: 15rem;
            opacity: 0.05;
            left: -60px;
            bottom: -60px;
            animation: float 10s ease-in-out infinite 2s;
        }
        
        .contact-info h3 {
            margin-bottom: 2rem;
            font-size: 2.5rem;
            position: relative;
            color: #22c55e;
            text-shadow: 0 0 20px rgba(34,197,94,0.6);
        }
        
        .contact-item {
            margin: 2rem 0;
            font-size: 1.3rem;
            animation: slideInLeft 0.6s ease;
            position: relative;
            padding: 1rem;
            background: rgba(34,197,94,0.05);
            border-radius: 10px;
            border-left: 4px solid #22c55e;
            transition: all 0.3s ease;
        }
        
        .contact-item:hover {
            background: rgba(34,197,94,0.15);
            transform: translateX(10px);
            border-left-width: 8px;
        }
        
        .contact-item strong {
            display: inline-block;
            width: 140px;
            color: #22c55e;
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #16a34a, #22c55e, #16a34a);
            background-size: 200% 200%;
            animation: gradientFlow 3s ease infinite;
            color: #0a1a0a;
            padding: 1.5rem 4rem;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.4rem;
            font-weight: bold;
            margin-top: 2rem;
            transition: all 0.4s ease;
            box-shadow: 0 10px 30px rgba(34,197,94,0.4),
                       0 0 30px rgba(34,197,94,0.3);
            position: relative;
            overflow: hidden;
            border: 3px solid rgba(255,255,255,0.3);
        }
        
        .cta-button::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255,255,255,0.5);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }
        
        .cta-button:hover::before {
            width: 400px;
            height: 400px;
        }
        
        .cta-button:hover {
            transform: scale(1.15);
            box-shadow: 0 20px 50px rgba(34,197,94,0.6),
                       0 0 60px rgba(34,197,94,0.5);
            border-color: rgba(255,255,255,0.6);
        }
        
        .map {
            margin-top: 3rem;
            border-radius: 30px;
            overflow: hidden;
            height: 500px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.5),
                       0 0 40px rgba(34,197,94,0.3);
            animation: fadeInUp 1s ease;
            border: 3px solid rgba(34,197,94,0.3);
        }
        
        .services-list {
            background: linear-gradient(135deg, rgba(34,197,94,0.1) 0%, rgba(255,255,255,0.05) 100%);
            padding: 3rem;
            border-radius: 20px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.3);
            border: 2px solid rgba(34,197,94,0.2);
            backdrop-filter: blur(10px);
        }
        
        .services-list ul {
            list-style: none;
        }
        
        .services-list li {
            font-size: 1.3rem;
            padding: 1.5rem;
            margin: 1rem 0;
            background: linear-gradient(90deg, rgba(34,197,94,0.15), rgba(34,197,94,0.05));
            border-radius: 15px;
            border-left: 5px solid #22c55e;
            transition: all 0.4s ease;
            animation: slideInLeft 0.5s ease;
            color: #e0e0e0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .services-list li:hover {
            transform: translateX(20px) scale(1.02);
            background: linear-gradient(90deg, #22c55e, #16a34a);
            color: #0a1a0a;
            box-shadow: 0 10px 30px rgba(34,197,94,0.5);
            border-left-width: 10px;
            font-weight: bold;
        }

        .pricing-table {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .price-card {
            background: linear-gradient(135deg, rgba(34,197,94,0.1) 0%, rgba(255,255,255,0.05) 100%);
            border-radius: 20px;
            padding: 2.5rem;
            text-align: center;
            border: 2px solid rgba(34,197,94,0.3);
            transition: all 0.5s ease;
            position: relative;
            overflow: hidden;
        }

        .price-card:hover {
            transform: translateY(-10px) scale(1.05);
            border-color: #22c55e;
            box-shadow: 0 20px 50px rgba(34,197,94,0.4);
        }

        .price-card h3 {
            color: #22c55e;
            font-size: 1.8rem;
            margin-bottom: 1rem;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }

        .price {
            font-size: 3rem;
            color: #fff;
            font-weight: bold;
            margin: 1.5rem 0;
            text-shadow: 0 0 20px rgba(34,197,94,0.5);
        }

        .price-features {
            list-style: none;
            margin: 1.5rem 0;
        }

        .price-features li {
            color: #e0e0e0;
            padding: 0.5rem;
            margin: 0.5rem 0;
        }
        
        footer {
            background: linear-gradient(135deg, #0a1a0a 0%, #1a3e1a 50%, #0a1a0a 100%);
            color: white;
            text-align: center;
            padding: 4rem;
            margin-top: 5rem;
            position: relative;
            overflow: hidden;
            border-top: 3px solid #22c55e;
            box-shadow: 0 -20px 60px rgba(0,0,0,0.5),
                       0 0 60px rgba(34,197,94,0.2);
        }
        
        footer::before {
            content: '🏍️';
            position: absolute;
            font-size: 15rem;
            opacity: 0.03;
            left: 5%;
            animation: float 10s ease-in-out infinite;
        }
        
        footer::after {
            content: '⚡';
            position: absolute;
            font-size: 15rem;
            opacity: 0.03;
            right: 5%;
            animation: float 10s ease-in-out infinite 3s;
        }
        
        footer p {
            position: relative;
            z-index: 2;
            color: #22c55e;
            text-shadow: 0 0 10px rgba(34,197,94,0.5);
        }

        .scroll-to-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: linear-gradient(135deg, #22c55e, #16a34a);
            color: #0a1a0a;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            cursor: pointer;
            opacity: 0;
            transition: all 0.3s ease;
            z-index: 999;
            box-shadow: 0 5px 20px rgba(34,197,94,0.5);
        }

        .scroll-to-top.visible {
            opacity: 1;
        }

        .scroll-to-top:hover {
            transform: translateY(-5px) scale(1.1);
            box-shadow: 0 10px 30px rgba(34,197,94,0.7);
        }

        .reservation-form {
            background: linear-gradient(135deg, rgba(34,197,94,0.1) 0%, rgba(255,255,255,0.05) 100%);
            padding: 3rem;
            border-radius: 20px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.3);
            border: 2px solid rgba(34,197,94,0.2);
            backdrop-filter: blur(10px);
            max-width: 900px;
            margin: 0 auto;
        }

        .form-row {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group.full-width {
            grid-column: 1 / -1;
        }

        .form-group label {
            color: #22c55e;
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            font-weight: 500;
            text-shadow: 0 0 5px rgba(34,197,94,0.3);
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            padding: 1rem;
            border: 2px solid rgba(34,197,94,0.3);
            border-radius: 10px;
            background: rgba(26,62,26,0.8);
            color: #e0e0e0;
            font-size: 1rem;
            font-family: inherit;
            transition: all 0.3s ease;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #22c55e;
            background: rgba(26,62,26,0.9);
            box-shadow: 0 0 20px rgba(34,197,94,0.3);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 80px;
        }

        .submit-button {
            width: 100%;
            padding: 1.5rem;
            background: linear-gradient(135deg, #16a34a, #22c55e, #16a34a);
            background-size: 200% 200%;
            animation: gradientFlow 3s ease infinite;
            color: #0a1a0a;
            font-size: 1.3rem;
            font-weight: bold;
            border: 3px solid rgba(255,255,255,0.3);
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.4s ease;
            box-shadow: 0 10px 30px rgba(34,197,94,0.4);
            margin-top: 2rem;
            position: relative;
            overflow: hidden;
        }

        .submit-button::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255,255,255,0.5);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }

        .submit-button:hover::before {
            width: 500px;
            height: 500px;
        }

        .submit-button:hover {
            transform: scale(1.05);
            box-shadow: 0 20px 50px rgba(34,197,94,0.6);
            border-color: rgba(255,255,255,0.6);
        }

        .submit-button:active {
            transform: scale(0.98);
        }
        
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }

            header {
                padding: 8rem 1rem 4rem;
            }

            header h1 {
                font-size: 2.5rem;
            }

            .hero-stats {
                gap: 1rem;
            }

            .stat-number {
                font-size: 2rem;
            }
            
            .features, .motos-gallery, .offers-grid {
                grid-template-columns: 1fr;
            }
            
            .section h2 {
                font-size: 2rem;
            }
            
            .section {
                padding: 2rem 1rem;
            }

            .pricing-table {
                grid-template-columns: 1fr;
            }

            .form-row {
                grid-template-columns: 1fr;
            }

            .reservation-form {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <nav>
        <div class="nav-container">
            <div class="logo">⚡ EBIKE AGADIR</div>
            <ul>
                <li><a href="#motos">Nos Motos</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#tarifs">Tarifs</a></li>
                <li><a href="#reservation">Réserver</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <header>
        <h1>⚡ LOCATION MOTOS ÉLECTRIQUES ⚡</h1>
        <p>Votre Mobilité Premium à Agadir Tikiouine</p>
        <div class="hero-stats">
            <div class="stat-item">
                <div class="stat-number">100%</div>
                <div class="stat-label">Écologique</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">100km</div>
                <div class="stat-label">Autonomie</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">24/7</div>
                <div class="stat-label">Support</div>
            </div>
        </div>
    </header>

    <div class="container">
        <section class="section" id="motos">
            <h2>NOS MOTOS ÉLECTRIQUES PREMIUM</h2>
            <div class="motos-gallery">
                <div class="moto-card">
                    <div class="moto-badge">POPULAIRE</div>
                    <img src="images/bike1.jpg" alt="Moto Électrique Grise">
                    <div class="moto-info">
                        <h3>🏍️ MOTO ÉLECTRIQUE SPORT</h3>
                        <p>Performance Extrême • Autonomie 100 km • Design Futuriste Premium</p>
                    </div>
                </div>
                <div class="moto-card">
                    <div class="moto-badge">NOUVEAU</div>
                    <img src="images/bike2.jpg" alt="Scooter Électrique Blanc">
                    <div class="moto-info">
                        <h3>🛵 SCOOTER ÉLECTRIQUE LUXE</h3>
                        <p>Confort Ultime • Autonomie 80 km • Élégance & Technologie</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>POURQUOI NOUS CHOISIR ?</h2>
            <div class="features">
                <div class="feature-card">
                    <h3>🌱 100% ÉCOLOGIQUE</h3>
                    <p>Zéro émission, énergie propre pour un environnement préservé et un futur durable</p>
                </div>
                <div class="feature-card">
                    <h3>💰 ULTRA ÉCONOMIQUE</h3>
                    <p>Prix imbattables, coûts réduits - Économisez jusqu'à 90% sur vos déplacements</p>
                </div>
                <div class="feature-card">
                    <h3>🔋 HAUTE PERFORMANCE</h3>
                    <p>Autonomie exceptionnelle jusqu'à 100 km - Explorez Agadir sans limites</p>
                </div>
                <div class="feature-card">
                    <h3>🛡️ SÉCURITÉ MAXIMALE</h3>
                    <p>Véhicules neufs premium, entretien parfait, assurance tous risques incluse</p>
                </div>
            </div>
        </section>

        <section class="section" id="services">
            <h2>NOS SERVICES PREMIUM</h2>
            <div class="services-list">
                <ul>
                    <li>⏱️ LOCATION ULTRA FLEXIBLE: Horaire, Journée, Semaine ou Mois</li>
                    <li>🪖 ÉQUIPEMENTS PREMIUM: Casques & Accessoires Haut de Gamme Fournis</li>
                    <li>🚚 LIVRAISON VIP: Gratuite à Votre Hôtel ou Domicile</li>
                    <li>📚 FORMATION COMPLÈTE: Cours Personnalisé pour Tous Niveaux</li>
                    <li>🔧 ASSISTANCE 24/7: Support Technique Expert à Tout Moment</li>
                    <li>📱 APPLICATION EXCLUSIVE: Suivi GPS & Gestion en Temps Réel</li>
                </ul>
            </div>
        </section>

        <section class="section" id="tarifs">
            <h2>NOS TARIFS COMPÉTITIFS</h2>
            <div class="pricing-table">
                <div class="price-card">
                    <h3>⏱️ HORAIRE</h3>
                    <div class="price">150 DH</div>
                    <ul class="price-features">
                        <li>✓ 1 heure de liberté</li>
                        <li>✓ Casque inclus</li>
                        <li>✓ Assurance comprise</li>
                    </ul>
                </div>
                <div class="price-card">
                    <h3>☀️ JOURNÉE</h3>
                    <div class="price">500 DH</div>
                    <ul class="price-features">
                        <li>✓ 24 heures complètes</li>
                        <li>✓ Tout équipement inclus</li>
                        <li>✓ Support prioritaire</li>
                    </ul>
                </div>
                <div class="price-card">
                    <h3>📅 SEMAINE</h3>
                    <div class="price">2800 DH</div>
                    <ul class="price-features">
                        <li>✓ 7 jours d'aventure</li>
                        <li>✓ Livraison gratuite</li>
                        <li>✓ GPS premium offert</li>
                    </ul>
                </div>
                <div class="price-card">
                    <h3>📆 MOIS</h3>
                    <div class="price">9000 DH</div>
                    <ul class="price-features">
                        <li>✓ 30 jours de mobilité</li>
                        <li>✓ Meilleur rapport qualité/prix</li>
                        <li>✓ Service VIP complet</li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="section">
            <h2>INCLUS DANS VOTRE LOCATION PREMIUM</h2>
            <div class="offers-grid">
                <div class="offer-card">
                    <img src="images/casque.jpg" alt="Casque">
                    <div class="offer-content">
                        <h3>🪖 CASQUE PREMIUM</h3>
                        <p>Casque haute protection certifié inclus</p>
                    </div>
                </div>
                <div class="offer-card">
                    <img src="images/assurance.jpg" alt="Assurance">
                    <div class="offer-content">
                        <h3>🛡️ ASSURANCE COMPLÈTE</h3>
                        <p>Couverture tous risques garantie</p>
                    </div>
                </div>
                <div class="offer-card">
                    <img src="images/gps.jpg" alt="GPS">
                    <div class="offer-content">
                        <h3>📱 SUPPORT GPS PRO</h3>
                        <p>Navigation intelligente intégrée</p>
                    </div>
                </div>
                <div class="offer-card">
                    <img src="images/livraison.jpg" alt="Livraison">
                    <div class="offer-content">
                        <h3>🚚 LIVRAISON VIP</h3>
                        <p>Service de conciergerie premium</p>
                    </div>
                </div>
                <div class="offer-card">
                    <img src="images/recharge.jpg" alt="Recharge">
                    <div class="offer-content">
                        <h3>⚡ ÉNERGIE MAXIMALE</h3>
                        <p>Batterie 100% chargée garantie</p>
                    </div>
                </div>
                <div class="offer-card">
                    <img src="images/assistance.jpg" alt="Assistance">
                    <div class="offer-content">
                        <h3>🔧 ASSISTANCE 24/7</h3>
                        <p>Support expert à tout moment</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section" id="reservation">
            <h2>FORMULAIRE DE RÉSERVATION</h2>
            <div class="reservation-form">
                <form id="bookingForm">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="nom">👤 Nom Complet *</label>
                            <input type="text" id="nom" name="nom" required>
                        </div>
                        <div class="form-group">
                            <label for="telephone">📱 Téléphone *</label>
                            <input type="tel" id="telephone" name="telephone" required>
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="email">✉️ Email</label>
                            <input type="email" id="email" name="email">
                        </div>
                        <div class="form-group">
                            <label for="ville">📍 Ville</label>
                            <input type="text" id="ville" name="ville">
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="moto">🏍️ Type de Moto *</label>
                            <select id="moto" name="moto" required>
                                <option value="">Choisissez votre moto...</option>
                                <option value="Moto Électrique Sport">🏍️ Moto Électrique Sport</option>
                                <option value="Scooter Électrique Luxe">🛵 Scooter Électrique Luxe</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="duree">⏱️ Durée de Location *</label>
                            <select id="duree" name="duree" required>
                                <option value="">Choisissez la durée...</option>
                                <option value="Horaire - 150 DH">⏱️ Horaire - 150 DH</option>
                                <option value="Journée - 500 DH">☀️ Journée - 500 DH</option>
                                <option value="Semaine - 2800 DH">📅 Semaine - 2800 DH</option>
                                <option value="Mois - 9000 DH">📆 Mois - 9000 DH</option>
                            </select>
                        </div>
                    </div>

                    <div class="form-row">
                        <div class="form-group">
                            <label for="date">📅 Date de Début *</label>
                            <input type="date" id="date" name="date" required>
                        </div>
                        <div class="form-group">
                            <label for="heure">🕐 Heure de Début *</label>
                            <input type="time" id="heure" name="heure" required>
                        </div>
                    </div>

                    <div class="form-group full-width">
                        <label for="livraison">🚚 Livraison</label>
                        <select id="livraison" name="livraison">
                            <option value="Non">Non - Je récupère sur place</option>
                            <option value="Oui">Oui - Livraison à mon adresse (Gratuit)</option>
                        </select>
                    </div>

                    <div class="form-group full-width" id="adresseGroup" style="display: none;">
                        <label for="adresse">📍 Adresse de Livraison</label>
                        <textarea id="adresse" name="adresse" rows="2" placeholder="Entrez l'adresse complète de livraison..."></textarea>
                    </div>

                    <div class="form-group full-width">
                        <label for="message">💬 Message / Demandes Spéciales</label>
                        <textarea id="message" name="message" rows="4" placeholder="Ajoutez vos commentaires ou demandes spéciales..."></textarea>
                    </div>

                    <button type="submit" class="submit-button">
                        📲 ENVOYER LA RÉSERVATION VIA WHATSAPP
                    </button>
                </form>
            </div>
        </section>

        <section class="section" id="contact">
            <h2>CONTACTEZ-NOUS</h2>
            <div class="contact-info">
                <h3>📍 NOUS TROUVER</h3>
                <div class="contact-item">
                    <strong>📍 ADRESSE:</strong> Tikiouine, Agadir, Maroc
                </div>
                <div class="contact-item">
                    <strong>📞 TÉLÉPHONE:</strong> +212 774 180 258
                </div>
                <div class="contact-item">
                    <strong>✉️ EMAIL:</strong> azizbousalem239@gmail.com
                </div>
                <div class="contact-item">
                    <strong>🕐 HORAIRES:</strong> Lundi - Vendredi: 08h00 - 19h00
                </div>
                
                <h3 style="margin-top: 3rem; text-align: center;">
                    <a href="#reservation" class="cta-button">📞 RÉSERVEZ MAINTENANT</a>
                </h3>
            </div>
            
            <div class="map">
                <iframe 
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d27525.685424238084!2d-9.639999!3d30.427755!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xdb3b6e8c7b3b3b3b%3A0x3b3b3b3b3b3b3b3b!2sTikiouine%2C%20Agadir%2080000!5e0!3m2!1sfr!2sma!4v1234567890"
                    width="100%" 
                    height="100%" 
                    style="border:0;" 
                    allowfullscreen="" 
                    loading="lazy"
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
        </section>
    </div>

    <div class="scroll-to-top" id="scrollTop">↑</div>

    <footer>
        <p style="font-size: 1.4rem; margin-bottom: 1rem; font-weight: bold;">⚡ LOCATION MOTOS ÉLECTRIQUES AGADIR ⚡</p>
        <p style="font-size: 1.2rem;">&copy; 2026 - Tous Droits Réservés</p>
        <p style="margin-top: 1.5rem; font-size: 1.3rem;">🌍 MOBILITÉ VERTE • AVENIR DURABLE • EXCELLENCE PREMIUM 🏍️</p>
    </footer>

    <script>
        // WhatsApp number
        const whatsappNumber = '212774180258';

        // Show/hide delivery address field
        const livraisonSelect = document.getElementById('livraison');
        const adresseGroup = document.getElementById('adresseGroup');

        livraisonSelect.addEventListener('change', function() {
            if (this.value === 'Oui') {
                adresseGroup.style.display = 'block';
            } else {
                adresseGroup.style.display = 'none';
            }
        });

        // Handle form submission
        document.getElementById('bookingForm').addEventListener('submit', function(e) {
            e.preventDefault();

            // Get form values
            const nom = document.getElementById('nom').value;
            const telephone = document.getElementById('telephone').value;
            const email = document.getElementById('email').value;
            const ville = document.getElementById('ville').value;
            const moto = document.getElementById('moto').value;
            const duree = document.getElementById('duree').value;
            const date = document.getElementById('date').value;
            const heure = document.getElementById('heure').value;
            const livraison = document.getElementById('livraison').value;
            const adresse = document.getElementById('adresse').value;
            const message = document.getElementById('message').value;

            // Format WhatsApp message
            let whatsappMessage = `🏍️ *NOUVELLE RÉSERVATION MOTO ÉLECTRIQUE* ⚡\n\n`;
            whatsappMessage += `👤 *Nom:* ${nom}\n`;
            whatsappMessage += `📱 *Téléphone:* ${telephone}\n`;
            if (email) whatsappMessage += `✉️ *Email:* ${email}\n`;
            if (ville) whatsappMessage += `📍 *Ville:* ${ville}\n`;
            whatsappMessage += `\n🏍️ *DÉTAILS DE LA RÉSERVATION:*\n`;
            whatsappMessage += `• *Moto:* ${moto}\n`;
            whatsappMessage += `• *Durée:* ${duree}\n`;
            whatsappMessage += `• *Date:* ${date}\n`;
            whatsappMessage += `• *Heure:* ${heure}\n`;
            whatsappMessage += `\n🚚 *LIVRAISON:* ${livraison}\n`;
            if (livraison === 'Oui' && adresse) {
                whatsappMessage += `📍 *Adresse:* ${adresse}\n`;
            }
            if (message) {
                whatsappMessage += `\n💬 *Message:*\n${message}\n`;
            }
            whatsappMessage += `\n✅ Merci de confirmer ma réservation!`;

            // Encode message for URL
            const encodedMessage = encodeURIComponent(whatsappMessage);

            // Open WhatsApp with the message
            window.open(`https://wa.me/${whatsappNumber}?text=${encodedMessage}`, '_blank');

            // Optional: Reset form after submission
            setTimeout(() => {
                if (confirm('Votre réservation a été envoyée via WhatsApp. Voulez-vous réinitialiser le formulaire?')) {
                    this.reset();
                    adresseGroup.style.display = 'none';
                }
            }, 1000);
        });

        // Scroll to top button
        const scrollTopBtn = document.getElementById('scrollTop');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                scrollTopBtn.classList.add('visible');
            } else {
                scrollTopBtn.classList.remove('visible');
            }
        });
        
        scrollTopBtn.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Smooth scrolling for nav links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(50px)';
            section.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            observer.observe(section);
        });
    </script>
</body>
</html>
