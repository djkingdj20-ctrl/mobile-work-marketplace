# Mobile Work Marketplace

Mobile-first marketplace MVP: user accounts, tasks, submissions, admin approval, wallet, withdrawals, and business task requests.

## Run
1. `npm install`
2. Set `JWT_SECRET` in the environment.
3. `npm start`
4. Open the service URL.

## Admin
For safety, the app does not create a public admin signup. To make the first admin, register a normal account and then change its `role` to `admin` in `data/database.json` after the first run. In production, use a proper admin provisioning flow and managed database.

## Important
The withdrawal feature creates admin-reviewed payout requests; it does not itself transfer real money. A real payout provider, KYC/compliance flow, fraud controls, and a persistent managed database are required before public launch.
