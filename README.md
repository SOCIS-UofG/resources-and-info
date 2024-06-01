# Resources and Info
Some resources and information regarding making changes and contributing to the website.

## Resources
### Architecture Resources
Below are some resources that you can review regarding how the socis website works.

1. Sub-domain Flowchart: https://app.eraser.io/workspace/1GB8xUB93YVxIcvQwgqp?origin=share

### Development resources
1. Prisma: [Fireship](https://www.youtube.com/watch?v=rLRIB6AF2Dg)
2. tRPC: [Fireship](https://www.youtube.com/watch?v=0DyAyLdVW0I) or [Jack Herrington](https://www.youtube.com/watch?v=qCLV0Iaq9zU)
3. Next.js: [Fireship](https://www.youtube.com/watch?v=Sklc_fQBmcs) or the documentation can be found [here](https://nextjs.org/docs)

## How to Contribute
### Cloning the repository
First, clone the repository using `git clone {repository .git url}`

### Verify the branch (important!)
Before you start editing, make sure you're on the `dev` branch and that you're on the latest version! Run `git pull` to pull all changes before making new ones!

### Creating a new branch
If you're making changes to this repo, copy/paste the following commands when you're making your `first` commit:

```
git checkout -b "your-name/feature"
git add .
git commit -m "New Feature"
git push --set-upstream origin "your-name/feature"
git checkout main
```

REPLACE `your-name/feature` with your name and the feature you're adding! 

> If it's not your first commit, use `git push` rather than `git push --set-upstream origin your-name/feature`

### Creating a pull request
Then head over to the GitHub repo online and create a pull request from the branch you just created.

After the first commit, you don't need to copy/paste the above again, you can make commits as usual.

### Adding a reviewer
Tell someone who is in the `Admin` team to review the code and merge the pull request. You can manually add a reviewer if you'd like.

# Some To-dos
Some to-dos. These were last updated May 2024.

- [ ] Convert `auth.socis.ca` to use JWT for sign up link and password reset link (**THIS IS VERY IMPORTANT**)


- [ ] Convert `<form>`'s to `react-hook-form` and `zod`
- [ ] Fix UI: Padding, more responsive on mobile, etc.
- [ ] Migrate from Vercel Blob Storage to AWS S3 or another S3 provider (Vercel’s blob storage limits are too low)
- [ ] Clean up the backend — i’m sure if you look around (especially in the account.socis.ca page) you’ll find some problems
- [ ] Better and more uniform input validation (on both the frontend and backend; this is similar to the `zod` and `react-hook-form` implementation).
- [ ] Better error handling and error messages.
- [ ] Better status handling (loading screens, errors, etc.)
- [ ] store.socis.ca and stripe implementation
- [ ] hardware checkout system
- [ ] socis.ca/about page needs a better design (most pages do also, get a designer to help maybe)

- [ ] Implement `prisma.$transaction` for deleting users from the database and their profile photos from blob storage.

## Final Notes (from Tristan)
Basically try to clean up the UI and the code. I'm sure there's a lot of bugs, you just need to play around to find them. If you ever need access to the database (Supabase, PostgreSQL), shoot me a DM on Discord @ realtristan

All the best and have fun coding!
