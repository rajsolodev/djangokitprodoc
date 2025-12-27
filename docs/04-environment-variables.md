# Environment Variables

Create a `.env` file in the project root.

## Django

DEBUG=True
SECRET_KEY=your-secret-key
ALLOWED_HOSTS=localhost,127.0.0.1

## Database

DATABASE_URL=postgres://user:password@localhost:5432/dbname

## Payment Providers

DODO_API_KEY=your-dodo-key
STRIPE_SECRET_KEY=your-stripe-key

## Email (optional)

EMAIL_HOST=smtp.gmail.com
EMAIL_HOST_USER=your-email
EMAIL_HOST_PASSWORD=app-password

## Notes

- Never commit `.env`
- Restart server after changing env values
- Use separate keys for production
