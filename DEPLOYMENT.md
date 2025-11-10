# Deployment Configuration

## Supabase Configuration
Replace these values in index.html:

```javascript
// Current placeholders (REPLACE THESE)
const supabaseUrl = 'YOUR_SUPABASE_URL';
const supabaseKey = 'YOUR_SUPABASE_ANON_KEY';

// Example of what they should look like:
const supabaseUrl = 'https://your-project-ref.supabase.co';
const supabaseKey = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...';
```

## CORS Settings in Supabase
Add these domains to your Supabase project settings:

1. Go to Supabase Dashboard → Settings → API
2. Add to "CORS origins":
   - `http://localhost:3000` (for local development)
   - `http://localhost:8000` (for local development)
   - `https://yourusername.github.io` (for GitHub Pages)
   - `https://your-custom-domain.com` (if using custom domain)

## Database Setup
Import the following files to your Supabase project:
1. Schema SQL file (table structure)
2. RPC functions SQL file
3. Sample data (optional)

## Security Checklist
- [ ] Replace default Supabase credentials
- [ ] Set up Row Level Security (RLS) policies
- [ ] Configure proper CORS origins
- [ ] Test all database connections
- [ ] Verify user authentication flows

## Post-Deployment Testing
- [ ] User login/registration
- [ ] Project creation and selection
- [ ] CSI hierarchy navigation
- [ ] Code generation
- [ ] Export functionality
- [ ] Database read/write operations
