# twin-films-web

### To Start
`npm install` --> installs everything from package-lock

`npm run dev` --> dev server start


### General Notes

AWS' integration with React involved some nuance. The following should be helpful for future AWS/React project deployments: 

Once you've verified that the website works via `npm run dev`, you should then run `npm run build`. Running `npm run build` creates a build output directory that (as of this version of react) seems to default to being named `dist`. Once you have an output directory, you should specify its path in AWS' App build specification. You can do this by modifying the `baseDirectory` tag in the virtually hosted `amplify.yml` file. The `amplify.yml` file is editable by navigating to [ App settings > Build settings > App build specification ] on the AWS console.
