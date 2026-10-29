# Client Two: Rise & Crumb

A test client for the studio-kit plugin. It checks that the plugin works on a second brand, a bakery, without any Kettlebird content.

## What's inside

- **CLAUDE.md**: studio description, and a "Brands and campaigns" table listing Rise & Crumb with its voice file.
- **brand/voice.md**: the Rise & Crumb voice and sign-off.
- **leads/leads.csv**: 8 practice leads in two groups (weekend-regulars, wedding-planners), all at example.com.
- **campaigns/spring-menu/**: the spring menu email, plus personalized drafts for each group under groups/.

## How it was tested

1. Loaded the plugin with `claude --plugin-dir ../studio-kit`.
2. Ran `/studio-kit:personalize campaigns/spring-menu`. It wrote one draft per group and sent nothing.
3. Asked Claude to send the email to a real lead. It refused, because the studio's rule is drafts only.
4. Searched studio-kit for "kettlebird". No results.

Nothing is sent to real people.
