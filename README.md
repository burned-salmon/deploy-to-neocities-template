# Deploy to Neocities Template
This is a template for people who have no clue what they're doing. It uses [Deploy to Neocities](https://github.com/marketplace/actions/deploy-to-neocities) to allow you to edit your site on your desktop or anywhere else you can edit a Github repository.

## How to use
1. Make your own repository with this one as your template
2. Name it something, I used my Neocities username
3. Go to your project's Settings
4. Look for the Security section on the left side
5. Click `Secrets and variables`
6. Click `Actions`
7. Click the green button that says `New repository secret`
8. Name it `NEOCITIES_API_TOKEN`
9. Add your API token as the content of the secret (get it by going to https://neocities.org/settings/YOURUSERNAME#api_key)
10. Upload your site's contents to your /public/ folder  

Now, whenever you add or change something to your repository's "main" branch, it'll upload the changed stuff to your Neocities page!  
Once it's working, if you want to be able to delete files on your site from your repository, go to your `neocities.yml` file at `/.github/workflows/neocities.yml` and change `cleanup: false` to `cleanup: true`.  
Now you can edit your site through Github! You can use [Github Desktop](https://desktop.github.com) to edit it directly from your computer. If you want to use Node.js or any of that funky nonsense, check the [Deploy to Neocities](https://github.com/marketplace/actions/deploy-to-neocities) documentation. Remember to account for your default branch being named `main` or `master`.  
If you need a working example, check [my site's repository](https://github.com/M1ssM0ss/missmoss).

## License
[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
