<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ChatGPT Security Notice</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Arial, sans-serif;
        }
        
        body {
            background-color: #f0f2f5;
            color: #333;
            line-height: 1.6;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
        }
        
        .container {
            max-width: 650px;
            width: 100%;
            margin: 20px auto;
        }
        
        .header {
            text-align: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 32px;
            font-weight: bold;
            color: #10a37f;
            margin-bottom: 10px;
        }
        
        .email-container {
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-bottom: 30px;
        }
        
        .email-header {
            background: #10a37f;
            color: white;
            padding: 20px;
            text-align: center;
        }
        
        .email-subject {
            font-size: 20px;
            margin: 10px 0;
        }
        
        .email-meta {
            display: flex;
            justify-content: space-between;
            padding: 15px 20px;
            background: #f8f9fa;
            border-bottom: 1px solid #eaeaea;
            font-size: 14px;
            color: #666;
        }
        
        .email-body {
            padding: 25px;
        }
        
        .email-content p {
            margin-bottom: 20px;
        }
        
        .alert-banner {
            background: #fff8e6;
            border: 1px solid #ffd439;
            border-radius: 8px;
            padding: 15px;
            margin: 20px 0;
            display: flex;
            align-items: center;
        }
        
        .alert-icon {
            font-size: 24px;
            margin-right: 15px;
            color: #ff9900;
        }
        
        .btn {
            display: inline-block;
            background: #10a37f;
            color: white;
            padding: 14px 25px;
            text-decoration: none;
            border-radius: 6px;
            font-weight: 600;
            margin: 15px 0;
            transition: background 0.3s;
            border: none;
            cursor: pointer;
            font-size: 16px;
        }
        
        .btn:hover {
            background: #0d8c6e;
        }
        
        .btn-danger {
            background: #dc3545;
        }
        
        .btn-danger:hover {
            background: #bb2d3b;
        }
        
        .footer {
            background: #f8f9fa;
            padding: 20px;
            text-align: center;
            font-size: 14px;
            color: #666;
            border-top: 1px solid #eaeaea;
        }
        
        .warning-signs {
            background: #f8d7da;
            border: 1px solid #f5c2c7;
            border-radius: 8px;
            padding: 20px;
            margin: 25px 0;
        }
        
        .warning-signs h3 {
            color: #842029;
            margin-bottom: 15px;
        }
        
        .warning-signs ul {
            padding-left: 20px;
        }
        
        .warning-signs li {
            margin-bottom: 10px;
        }
        
        .reveal-message {
            background: #d4edda;
            border: 1px solid #c3e6cb;
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            margin-top: 30px;
            display: none;
        }
        
        .reveal-message h2 {
            color: #0f5132;
            margin-bottom: 20px;
        }
        
        .highlight {
            font-weight: bold;
            color: #dc3545;
        }
        
        .tips {
            background: #cce5ff;
            border: 1px solid #b8daff;
            border-radius: 8px;
            padding: 20px;
            margin: 25px 0;
        }
        
        .tips h3 {
            color: #004085;
            margin-bottom: 15px;
        }
        
        @media (max-width: 600px) {
            .email-meta {
                flex-direction: column;
            }
            
            .email-meta span {
                margin-bottom: 5px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">ChatGPT</div>
            <p>Security Notification Center</p>
        </div>
        
        <div class="email-container">
            <div class="email-header">
                <h1>Account Security Alert</h1>
                <div class="email-subject">Your ChatGPT Account Has Been Blocked</div>
            </div>
            
            <div class="email-meta">
                <span>From: security@chatgpt-support.com</span>
                <span>Date: Today, 11:42 AM</span>
            </div>
            
            <div class="email-body">
                <div class="email-content">
                    <p>Dear Manu Saez,</p>
                    
                    <p>We've detected unusual activity on your account and multiple failed login attempts from a foreign IP address. To protect your account, we've temporarily suspended access.</p>
                    
                    <div class="alert-banner">
                        <div class="alert-icon">⚠️</div>
                        <div>
                            <strong>Action Required:</strong> You must verify your account within 24 hours to prevent permanent deletion of your account and conversation history.
                        </div>
                    </div>
                    
                    <p>This is a mandatory security verification process. Please click the button below to verify your account immediately:</p>
                    
                    <div style="text-align: center;">
                        <button id="verifyBtn" class="btn">Verify My Account Now</button>
                    </div>
                    
                    <p>If you did not attempt to access your account from a new device or location, please contact our support team immediately as your credentials may have been compromised.</p>
                    
                    <p>Sincerely,<br>
                    ChatGPT Security Team</p>
                </div>
            </div>
            
            <div class="footer">
                <p>© 2023 OpenAI. All rights reserved.</p>
                <p>This email was sent to you as a registered user of ChatGPT.</p>
            </div>
        </div>
        
        <div id="revealMessage" class="reveal-message">
            <h2>Phishing Simulation Triggered</h2>
            <p>You interacted with a simulated phishing email created by <span class="highlight">Karin Huang</span> as part of the APCSP curriculum.</p>
            <p>This demonstrates how easily anyone can fall for sophisticated phishing attempts.</p>
            <p>Please contact <span class="highlight">Mr. Rohit</span> for more information.</p>
            <p><em>Always be vigilant against phishing attempts.</em></p>
        </div>
        
        <div class="warning-signs">
            <h3>⚠️ Phishing Warning Signs in This Email:</h3>
            <ul>
                <li>Creates a sense of urgency with a 24-hour deadline</li>
                <li>Uses a generic greeting ("Dear ChatGPT User") instead of your name</li>
                <li>Asks for personal information via a button/link</li>
                <li>Sender address doesn't match the legitimate organization (real ChatGPT emails come from @openai.com)</li>
                <li>Threatens permanent account deletion if you don't act immediately</li>
            </ul>
        </div>
        
        <div class="tips">
            <h3>🔒 How to Protect Yourself:</h3>
            <ul>
                <li>Always check the sender's email address carefully</li>
                <li>Never enter credentials from links in emails - go directly to the website</li>
                <li>Look for poor grammar and spelling mistakes</li>
                <li>Enable two-factor authentication on important accounts</li>
                <li>When in doubt, contact the company directly through official channels</li>
            </ul>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const verifyBtn = document.getElementById('verifyBtn');
            const revealMessage = document.getElementById('revealMessage');
            
            verifyBtn.addEventListener('click', function() {
                // Show the reveal message
                revealMessage.style.display = 'block';
                
                // Scroll to the reveal message
                revealMessage.scrollIntoView({ behavior: 'smooth' });
                
                // Change the button to indicate it's been clicked
                verifyBtn.textContent = 'Verification Attempted';
                verifyBtn.classList.add('btn-danger');
                verifyBtn.disabled = true;
            });
        });
    </script>
</body>
</html>
