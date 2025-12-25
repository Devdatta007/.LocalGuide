# Contact Form Setup Instructions

Your contact form is currently configured to use **FormSubmit** - a free service that sends form submissions directly to your email.

## Setup Steps:

### 1. Replace Email Address
In `index.html`, find this line:
```html
<form class="contact-form" action="https://formsubmit.co/your-email@example.com" method="POST">
```

Replace `your-email@example.com` with your actual email address:
```html
<form class="contact-form" action="https://formsubmit.co/youremail@gmail.com" method="POST">
```

### 2. Verify Your Email (First Time Only)
1. Open your website in a browser
2. Fill out the contact form and submit it
3. FormSubmit will send a verification email to your address
4. Click the verification link in that email
5. After verification, all future form submissions will be sent to your email automatically

### 3. Features Included:
- ✅ Email notifications for every form submission
- ✅ Spam protection (captcha disabled for better UX)
- ✅ Professional table format for emails
- ✅ Custom subject line: "New message from Satara Guide website"
- ✅ Completely free - no signup required

## Alternative Options:

### Option 2: EmailJS (More Features)
If you want more control:
1. Sign up at https://www.emailjs.com/
2. Get your Service ID, Template ID, and Public Key
3. Follow their integration guide

### Option 3: Backend Server
For a professional setup:
- Use Node.js with Nodemailer
- Use PHP mail() function
- Use a contact form plugin if using WordPress

## Testing:
1. Replace the email address in the form action
2. Open index.html in your browser
3. Fill out and submit the form
4. Check your email inbox (and spam folder)

## Troubleshooting:
- **Not receiving emails?** Check your spam folder
- **Need verification?** Submit the form once to trigger verification email
- **Want custom redirect?** Add `<input type="hidden" name="_next" value="https://yoursite.com/thanks.html">`

## Current Configuration:
- Service: FormSubmit (https://formsubmit.co)
- Cost: Free
- Setup Time: 2 minutes
- Verification: Required (one-time)
