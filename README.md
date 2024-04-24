# Rails Password Validation Assessment

A Rails 7 assessment demonstrating matching password rules in the user model and a Stimulus-powered registration form.

## Validation contract

- Valid, unique email.
- Minimum password length.
- At least one lowercase letter, uppercase letter, digit, and special character.
- Matching password confirmation.

```bash
bundle install
rails db:create db:migrate
rails server
bundle exec rspec
```

The project originated as a Bark assessment and is presented with that scope. Controller and model specs cover the server behavior; client-side validation improves feedback but never replaces server enforcement. The app and specs were not run during review. Production authentication would additionally require secure password recovery, rate limits, session controls, email verification, and CSRF review.
