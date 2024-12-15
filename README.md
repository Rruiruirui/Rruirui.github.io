
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>我的简历</title>
        <style>
            :root {
                --color-white: #FFFFFF;
                --color-black: #000000;
                --color-darkgray: #333333;
                --color-gray: #5D5D5D;
                --color-lightgray: #999999;
                --color-text: var(--color-darkgray);
                --color-graytext: var(--color-gray);
                --color-lighttext: var(--color-lightgray);
                --color-awesome: #DC3522;
                --font-size-base: 16px;
                --spacing-unit: 1rem;
            }

            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
            }

            body {
                font-family: 'Source Sans Pro', sans-serif;
                font-size: var(--font-size-base);
                line-height: 1.5;
                color: var(--color-text);
                background: var(--color-white);
                padding: 2rem;
                max-width: 1200px;
                margin: 0 auto;
            }

            /* .cv-header {
                text-align: center;
                margin-bottom: 2rem;
            } */

            .cv-name {
                display: flex;
                justify-content: center;
                align-items: baseline;
                gap: 0.5rem;
                margin-bottom: 1rem;
            }

            .firstname {
                font-size: 2rem;
                font-weight: 300;
                color: var(--color-graytext);
            }

            .lastname {
                font-size: 2rem;
                font-weight: 700;
                color: var(--color-text);
            }

            .position {
                font-size: 0.9rem;
                text-transform: uppercase;
                color: var(--color-awesome);
                margin-bottom: 0.5rem;
            }

            .contact-info {
                font-size: 0.8rem;
                color: var(--color-lighttext);
            }

            .section {
                margin-bottom: 2rem;
            }

            .section-title {
                font-size: 1.25rem;
                font-weight: 700;
                color: var(--color-awesome);
                text-transform: uppercase;
                margin-bottom: 1rem;
                position: relative;
            }

            .section-title::after {
                content: '';
                position: absolute;
                left: 0;
                bottom: -0.25rem;
                width: 100%;
                height: 0.15rem;
                background-color: var(--color-awesome);
                opacity: 0.3;
            }

            .entry {
                margin-bottom: 1.5rem;
            }

            .entry-title {
                font-weight: 700;
                margin-bottom: 0.25rem;
            }
            .entry-title-small {
                font-weight: 500;
                margin-bottom: 0.25rem;
            }

            .entry-info {
                display: flex;
                justify-content: space-between;
                font-size: 0.9rem;
                color: var(--color-graytext);
                margin-bottom: 0.5rem;
            }

            .entry-description {
                font-size: 0.9rem;
                color: var(--color-text);
            }

            @media (max-width: 768px) {
                body {
                    padding: 1rem;
                }

                .entry-info {
                    flex-direction: column;
                    gap: 0.25rem;
                }
            }
            .blue-link {
                color: blue;
                text-decoration: none; /* 移除下划线 */
            }
            .blue-link:hover {
                text-decoration: underline; /* 悬停时显示下划线 */
            }
            .cv-header {
                text-align: center;
                margin-bottom: 2rem;
                position: relative;
                padding: 1rem;
            }

            .photo-container {
                width: 120px;
                height: 120px;
                position: absolute;
                overflow: hidden;
            }

            .photo-container.left {
                left: 0;
            }

            .photo-container.right {
                right: 0;
            }

            .photo-container.circle {
                border-radius: 50%;
            }

            .photo-container.rectangle {
                border-radius: 3px;
            }

            .photo-container.edge {
                border: 3px solid var(--color-awesome);
            }

            .photo-container img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }

            /* Adjust header layout when photo is present */
            .has-photo {
                padding-left: 140px; /* When photo is on the left */
            }

            .has-photo.photo-right {
                padding-left: 0;
                padding-right: 140px;
            }

            @media (max-width: 768px) {
                .cv-header {
                    padding: 0;
                }

                .photo-container {
                    position: relative;
                    margin: 0 auto 1rem auto;
                }

                .has-photo, .has-photo.photo-right {
                    padding: 0;
                }
            }
        </style>
    </head>
    <body>
        <header class="cv-header">
            <!-- Photo container with configurable options -->
            <div class="photo-container left circle edge">
                <!-- Replace src with actual photo path -->
                <img src="微信图片_20241210214030.jpg" alt="Profile Photo">
            </div>
            <div class="cv-name">
                <span class="firstname">任</span>
                <span class="lastname">庆蕊</span>
            </div>
            <div class="position">主修自动化专业 辅修人工智能专业</div>
            <div class="contact-info">
                📍 青岛科技大学, 山东省青岛市崂山区• 📱 (+86) 19854273396 • 📧 3620655370@qq.com
            </div>
        </header>

        <main>
            <section class="section">
                <h2 class="section-title">教育经历</h2>
                <div class="entry">
                    <h3 class="entry-title">青岛科技大学 (QUST)</h3>
                    <div class="entry-info">
                        <span>第一专业：自动化</span>
                        <span>青岛, 中国, 2023.9 - 2027.6</span>
                    </div>
                    <div class="entry-description">
                        主修有控制系统相关的过程控制、运动控制、检测技术、仿真与优化等
                    </div>
                </div>
                <div class="entry">
                    <h3 class="entry-title">青岛科技大学 (QUST)</h3>
                    <div class="entry-info">
                        <span>第二专业：人工智能</span>
                        <span>青岛, 中国, 2023.9 - 2027.6</span>
                    </div>
                    <div class="entry-description">
                        主修有python程序语言设计、网络爬虫与信息提取等
                    </div>
                </div>
            </section>


            <section class="section">
                <h2 class="section-title">个人信息</h2>
                <div class="entry">
                    <div class="entry-info">
                        <span>出生年月：2005.07</span>
                    </div>
                    <div class="entry-description">
                         <span>出生地：山东省聊城市</span>
                    </div>
                    <div class="entry-description">
                         <span>政治面貌：共青团员 </span>
                    </div>
                </div>
            </section>

            <section class="section">
                <h2 class="section-title">获奖经历</h2>
                <div class="entry">
                    <div class="entry-info">
                        <span>全国大学省英语竞赛二等奖</span>
                    </div>
                    <div class="entry-description">
                        <span>全国大学生数学建模竞赛省级三等奖</span>
                    </div>

        </main>
    </body>
</html>
