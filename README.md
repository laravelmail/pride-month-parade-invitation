# Pride Month Parade Invitation

A professional and inclusive invitation for a Pride Month Parade, suitable for the entertainment industry and non-profit organizations.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Entertainment, Non-Profit
- **Message Type:** Events
- **Tags:** celebration, pridemonth, parade

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/pride-month-parade-invitation.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/pride-month-parade-invitation/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.pride-month-parade-invitation',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
