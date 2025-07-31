<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>动漫宇宙 | 探索二次元世界</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #ff6b8b;
            --secondary: #6a5af9;
            --accent: #4deeea;
            --dark: #2a2438;
            --light: #f9f7fe;
        }

        body {
            background: linear-gradient(135deg, #1a1a2e, #16213e);
            color: var(--light);
            overflow-x: hidden;
        }

        /* 导航栏样式 */
        header {
            background: rgba(42, 36, 56, 0.85);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.3);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 2rem;
            font-weight: 800;
            background: linear-gradient(45deg, var(--accent), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            color: var(--light);
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            position: relative;
            transition: 0.3s;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 3px;
            background: var(--accent);
            transition: 0.3s;
            border-radius: 3px;
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .search-cart {
            display: flex;
            gap: 20px;
            align-items: center;
        }

        .search-cart i {
            font-size: 1.3rem;
            cursor: pointer;
            transition: 0.3s;
        }

        .search-cart i:hover {
            color: var(--accent);
            transform: scale(1.1);
        }

        /* 英雄区域样式 */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding-top: 80px;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1635189779577-555debfa2a0e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2000&q=80') no-repeat center/cover;
            opacity: 0.2;
            z-index: -1;
        }

        .hero-content {
            width: 60%;
            z-index: 1;
        }

        .hero h1 {
            font-size: 4.5rem;
            line-height: 1.1;
            margin-bottom: 20px;
            background: linear-gradient(45deg, var(--accent), var(--primary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .hero p {
            font-size: 1.4rem;
            margin-bottom: 40px;
            color: #e0d9ff;
            line-height: 1.6;
        }

        .cta-button {
            display: inline-block;
            padding: 15px 40px;
            background: linear-gradient(45deg, var(--secondary), var(--accent));
            color: white;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.2rem;
            border-radius: 50px;
            transition: 0.3s;
            box-shadow: 0 10px 20px rgba(106, 90, 249, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 25px rgba(106, 90, 249, 0.4);
        }

        .hero-image {
            position: absolute;
            right: -50px;
            bottom: -50px;
            width: 50%;
            max-width: 700px;
            filter: drop-shadow(0 20px 30px rgba(0, 0, 0, 0.4));
            animation: float 6s ease-in-out infinite;
        }

        /* 角色展示区域 */
        .section-title {
            text-align: center;
            font-size: 2.8rem;
            margin: 80px 0 50px;
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 5px;
            background: var(--accent);
            border-radius: 5px;
        }

        .characters {
            padding: 50px 0;
            background: rgba(26, 22, 46, 0.7);
        }

        .character-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }

        .character-card {
            background: rgba(42, 36, 56, 0.8);
            border-radius: 20px;
            overflow: hidden;
            transition: 0.4s;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            position: relative;
        }

        .character-card:hover {
            transform: translateY(-15px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        .character-img {
            height: 350px;
            width: 100%;
            overflow: hidden;
        }

        .character-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: 0.5s;
        }

        .character-card:hover .character-img img {
            transform: scale(1.1);
        }

        .character-info {
            padding: 20px;
        }

        .character-info h3 {
            font-size: 1.6rem;
            margin-bottom: 10px;
            color: var(--accent);
        }

        .character-info p {
            color: #c5c1e6;
            line-height: 1.6;
        }

        .character-tags {
            display: flex;
            gap: 10px;
            margin-top: 15px;
            flex-wrap: wrap;
        }

        .tag {
            background: rgba(77, 238, 234, 0.15);
            color: var(--accent);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        /* 新番推荐 */
        .anime-list {
            padding: 80px 0;
        }

        .anime-container {
            display: flex;
            gap: 40px;
            overflow-x: auto;
            padding: 30px 10px;
            scrollbar-width: thin;
            scrollbar-color: var(--accent) var(--dark);
        }

        .anime-container::-webkit-scrollbar {
            height: 8px;
        }

        .anime-container::-webkit-scrollbar-thumb {
            background: var(--accent);
            border-radius: 10px;
        }

        .anime-card {
            min-width: 280px;
            background: rgba(42, 36, 56, 0.8);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            transition: 0.3s;
        }

        .anime-card:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }

        .anime-cover {
            height: 380px;
            position: relative;
        }

        .anime-cover img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .anime-rating {
            position: absolute;
            top: 15px;
            right: 15px;
            background: rgba(255, 215, 0, 0.9);
            color: #000;
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: 700;
        }

        .anime-details {
            padding: 20px;
        }

        .anime-title {
            font-size: 1.4rem;
            margin-bottom: 10px;
            color: var(--accent);
        }

        .anime-meta {
            display: flex;
            justify-content: space-between;
            color: #a29cc0;
            margin-bottom: 15px;
            font-size: 0.9rem;
        }

        .anime-desc {
            color: #c5c1e6;
            line-height: 1.5;
            font-size: 0.95rem;
        }

        /* 新闻区域 */
        .news {
            padding: 80px 0;
            background: rgba(26, 22, 46, 0.7);
        }

        .news-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
        }

        .news-card {
            background: rgba(42, 36, 56, 0.8);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            transition: 0.3s;
            display: flex;
            flex-direction: column;
        }

        .news-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }

        .news-img {
            height: 220px;
        }

        .news-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .news-content {
            padding: 25px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .news-date {
            color: var(--accent);
            font-size: 0.9rem;
            margin-bottom: 10px;
        }

        .news-title {
            font-size: 1.4rem;
            margin-bottom: 15px;
            color: white;
        }

        .news-excerpt {
            color: #c5c1e6;
            line-height: 1.6;
            margin-bottom: 20px;
            flex-grow: 1;
        }

        .read-more {
            color: var(--accent);
            text-decoration: none;
            font-weight: 600;
            align-self: flex-start;
            transition: 0.3s;
        }

        .read-more:hover {
            text-decoration: underline;
        }

        /* 页脚样式 */
        footer {
            background: rgba(21, 16, 48, 0.95);
            padding: 70px 0 30px;
            position: relative;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-column h3 {
            font-size: 1.4rem;
            color: var(--accent);
            margin-bottom: 25px;
            position: relative;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--accent);
            border-radius: 3px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 15px;
        }

        .footer-links a {
            color: #b8b5d6;
            text-decoration: none;
            transition: 0.3s;
            display: flex;
            align-items: center;
        }

        .footer-links a:hover {
            color: var(--accent);
            transform: translateX(5px);
        }

        .footer-links i {
            margin-right: 10px;
            color: var(--accent);
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-icons a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            background: rgba(77, 238, 234, 0.1);
            border-radius: 50%;
            color: var(--accent);
            font-size: 1.3rem;
            transition: 0.3s;
        }

        .social-icons a:hover {
            background: var(--accent);
            color: var(--dark);
            transform: translateY(-5px);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #a29cc0;
            font-size: 0.95rem;
        }

        /* 动画效果 */
        @keyframes float {
            0% {
                transform: translateY(0px);
            }
            50% {
                transform: translateY(-20px);
            }
            100% {
                transform: translateY(0px);
            }
        }

        /* 响应式设计 */
        @media (max-width: 992px) {
            .hero-content {
                width: 100%;
                text-align: center;
            }
            
            .hero h1 {
                font-size: 3.5rem;
            }
            
            .hero-image {
                display: none;
            }
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .hero p {
                font-size: 1.2rem;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .character-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">
                    <i class="fas fa-dragon"></i>
                    <span>动漫宇宙</span>
                </div>
                <div class="nav-links">
                    <a href="#">首页</a>
                    <a href="#">动漫作品</a>
                    <a href="#">角色图鉴</a>
                    <a href="#">新番推荐</a>
                    <a href="#">动漫资讯</a>
                    <a href="#">社区</a>
                </div>
                <div class="search-cart">
                    <i class="fas fa-search"></i>
                    <i class="fas fa-user"></i>
                    <i class="fas fa-shopping-cart"></i>
                </div>
            </nav>
        </div>
    </header>

    <!-- 英雄区域 -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>探索无限精彩的二次元世界</h1>
                <p>汇聚全球优质动漫作品，发现你喜爱的角色，追踪最新动漫资讯，加入我们的动漫爱好者社区！</p>
                <a href="#" class="cta-button">立即探索 <i class="fas fa-arrow-right"></i></a>
            </div>
            <img src="https://images.unsplash.com/photo-1541562232579-512a21360020?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=800&q=80" alt="Anime Character" class="hero-image">
        </div>
    </section>

    <!-- 角色展示 -->
    <section class="characters">
        <div class="container">
            <h2 class="section-title">人气角色</h2>
            <div class="character-grid">
                <div class="character-card">
                    <div class="character-img">
                        <img src="https://images.unsplash.com/photo-1634142778880-c77aae08b9e2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Character 1">
                    </div>
                    <div class="character-info">
                        <h3>夜神月</h3>
                        <p>天才高中生，偶然获得死亡笔记后开始清除罪犯，试图创造新世界。</p>
                        <div class="character-tags">
                            <span class="tag">死亡笔记</span>
                            <span class="tag">主角</span>
                            <span class="tag">高智商</span>
                        </div>
                    </div>
                </div>
                
                <div class="character-card">
                    <div class="character-img">
                        <img src="https://images.unsplash.com/photo-1635189779577-555debfa2a0e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Character 2">
                    </div>
                    <div class="character-info">
                        <h3>御坂美琴</h3>
                        <p>学园都市最强电击使，代号"超电磁炮"，性格爽朗正义感强。</p>
                        <div class="character-tags">
                            <span class="tag">某科学的超电磁炮</span>
                            <span class="tag">Level 5</span>
                            <span class="tag">傲娇</span>
                        </div>
                    </div>
                </div>
                
                <div class="character-card">
                    <div class="character-img">
                        <img src="https://images.unsplash.com/photo-1547981609-4b6bf67db5dc?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Character 3">
                    </div>
                    <div class="character-info">
                        <h3>漩涡鸣人</h3>
                        <p>梦想成为火影的忍者，体内封印着九尾妖狐，拥有永不放弃的忍道。</p>
                        <div class="character-tags">
                            <span class="tag">火影忍者</span>
                            <span class="tag">主角</span>
                            <span class="tag">热血</span>
                        </div>
                    </div>
                </div>
                
                <div class="character-card">
                    <div class="character-img">
                        <img src="https://images.unsplash.com/photo-1541562232579-512a21360020?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Character 4">
                    </div>
                    <div class="character-info">
                        <h3>利威尔</h3>
                        <p>人类最强士兵，调查兵团兵长，战斗力超群但有着洁癖。</p>
                        <div class="character-tags">
                            <span class="tag">进击的巨人</span>
                            <span class="tag">兵长</span>
                            <span class="tag">阿克曼</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 新番推荐 -->
    <section class="anime-list">
        <div class="container">
            <h2 class="section-title">新番推荐</h2>
            <div class="anime-container">
                <div class="anime-card">
                    <div class="anime-cover">
                        <img src="https://images.unsplash.com/photo-1633356122544-f134324a6cee?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Anime 1">
                        <div class="anime-rating">9.8</div>
                    </div>
                    <div class="anime-details">
                        <h3 class="anime-title">鬼灭之刃 锻刀村篇</h3>
                        <div class="anime-meta">
                            <span>2023</span>
                            <span>11集</span>
                        </div>
                        <p class="anime-desc">炭治郎前往锻刀村寻找新的日轮刀，却遭遇上弦之鬼的袭击。霞柱与恋柱参战，展开激烈战斗。</p>
                    </div>
                </div>
                
                <div class="anime-card">
                    <div class="anime-cover">
                        <img src="https://images.unsplash.com/photo-1548802673-380ab8ebc7b7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Anime 2">
                        <div class="anime-rating">9.5</div>
                    </div>
                    <div class="anime-details">
                        <h3 class="anime-title">我推的孩子</h3>
                        <div class="anime-meta">
                            <span>2023</span>
                            <span>12集</span>
                        </div>
                        <p class="anime-desc">妇产科医生转生成偶像的孩子，在演艺圈揭开母亲死亡真相的故事。</p>
                    </div>
                </div>
                
                <div class="anime-card">
                    <div class="anime-cover">
                        <img src="https://images.unsplash.com/photo-1598520106830-8c45c2035460?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Anime 3">
                        <div class="anime-rating">9.2</div>
                    </div>
                    <div class="anime-details">
                        <h3 class="anime-title">咒术回战 第二季</h3>
                        <div class="anime-meta">
                            <span>2023</span>
                            <span>23集</span>
                        </div>
                        <p class="anime-desc">讲述五条悟的过去以及涩谷事变，咒术高专与咒灵全面开战。</p>
                    </div>
                </div>
                
                <div class="anime-card">
                    <div class="anime-cover">
                        <img src="https://images.unsplash.com/photo-1548802673-380ab8ebc7b7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Anime 4">
                        <div class="anime-rating">9.0</div>
                    </div>
                    <div class="anime-details">
                        <h3 class="anime-title">葬送的芙莉莲</h3>
                        <div class="anime-meta">
                            <span>2023</span>
                            <span>28集</span>
                        </div>
                        <p class="anime-desc">精灵魔法使芙莉莲在勇者死后踏上旅程，重新认识生命与时间的故事。</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 动漫新闻 -->
    <section class="news">
        <div class="container">
            <h2 class="section-title">动漫资讯</h2>
            <div class="news-grid">
                <div class="news-card">
                    <div class="news-img">
                        <img src="https://images.unsplash.com/photo-1635189779249-aaa7b7e55ce6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="News 1">
                    </div>
                    <div class="news-content">
                        <div class="news-date">2023年11月15日</div>
                        <h3 class="news-title">《进击的巨人》最终季完结篇创收视纪录</h3>
                        <p class="news-excerpt">历经十年的史诗巨作《进击的巨人》最终季完结篇播出后，在全球范围内引发观看热潮，创下动漫历史最高收视纪录...</p>
                        <a href="#" class="read-more">阅读更多 <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                
                <div class="news-card">
                    <div class="news-img">
                        <img src="https://images.unsplash.com/photo-1634128221889-82ed6efebfc3?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="News 2">
                    </div>
                    <div class="news-content">
                        <div class="news-date">2023年11月10日</div>
                        <h3 class="news-title">宫崎骏新作《你想活出怎样的人生》全球首映</h3>
                        <p class="news-excerpt">82岁动画大师宫崎骏时隔10年的新作《你想活出怎样的人生》在东京国际电影节全球首映，引发热烈反响...</p>
                        <a href="#" class="read-more">阅读更多 <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
                
                <div class="news-card">
                    <div class="news-img">
                        <img src="https://images.unsplash.com/photo-1638803040283-7a5ffd48dad5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="News 3">
                    </div>
                    <div class="news-content">
                        <div class="news-date">2023年11月5日</div>
                        <h3 class="news-title">2023年度动漫大奖揭晓</h3>
                        <p class="news-excerpt">2023年度动漫大奖结果公布，《咒术回战》获最佳动画，《赛博朋克：边缘行者》获最佳原创动画...</p>
                        <a href="#" class="read-more">阅读更多 <i class="fas fa-arrow-right"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>关于我们</h3>
                    <p style="color:#b8b5d6; line-height:1.6; margin-bottom:20px;">动漫宇宙是致力于为全球动漫爱好者提供最新资讯、作品推荐和交流平台的网站。我们分享优质内容，连接每一位热爱动漫的朋友。</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-weibo"></i></a>
                        <a href="#"><i class="fab fa-qq"></i></a>
                        <a href="#"><i class="fab fa-bilibili"></i></a>
                        <a href="#"><i class="fab fa-weixin"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>快速链接</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 首页</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 动漫作品</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 角色图鉴</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 新番时间表</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 动漫论坛</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>热门分类</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 热血冒险</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 科幻奇幻</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 恋爱校园</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 悬疑推理</a></li>
                        <li><a href="#"><i class="fas fa-chevron-right"></i> 治愈日常</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>联系我们</h3>
                    <ul class="footer-links">
                        <li><a href="#"><i class="fas fa-envelope"></i> contact@animeverse.com</a></li>
                        <li><a href="#"><i class="fas fa-phone"></i> +86 123 4567 8910</a></li>
                        <li><a href="#"><i class="fas fa-map-marker-alt"></i> 北京市朝阳区动漫产业园</a></li>
                        <li><a href="#"><i class="fas fa-headset"></i> 在线客服</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 动漫宇宙 AnimeVerse. 保留所有权利。 | 设计与开发 by AnimeFan Team</p>
            </div>
        </div>
    </footer>

    <script>
        // 简单的滚动效果增强
        document.addEventListener('DOMContentLoaded', function() {
            // 滚动时导航栏效果
            window.addEventListener('scroll', function() {
                const header = document.querySelector('header');
                if (window.scrollY > 50) {
                    header.style.background = 'rgba(26, 22, 46, 0.95)';
                    header.style.boxShadow = '0 5px 20px rgba(0, 0, 0, 0.4)';
                } else {
                    header.style.background = 'rgba(42, 36, 56, 0.85)';
                    header.style.boxShadow = '0 5px 20px rgba(0, 0, 0, 0.3)';
                }
            });
            
            // 卡片悬停效果增强
            const cards = document.querySelectorAll('.character-card, .anime-card, .news-card');
            cards.forEach(card => {
                card.addEventListener('mouseenter', function() {
                    this.style.zIndex = '10';
                });
                
                card.addEventListener('mouseleave', function() {
                    this.style.zIndex = '1';
                });
            });
            
            // 简单的搜索功能
            const searchIcon = document.querySelector('.fa-search');
            searchIcon.addEventListener('click', function() {
                const searchTerm = prompt('请输入搜索关键词:');
                if (searchTerm) {
                    alert(`正在搜索: ${searchTerm}\n（此功能为演示效果，实际网站需连接数据库）`);
                }
            });
        });
    </script>
</body>
</html>