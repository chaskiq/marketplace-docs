## Chaskiq AppStore

In order to sync our plugins with the Chaskiq AppStore you will need to download with your `license_key`, 

  + Add your `CHASKIQ_APPSTORE_KEY` to your env variables, if you are on development mode add it on `.env` file.
  + Run the download command to download your plugins `bundle exec rails packages:download`
  + To install the plugins you have downloaded run `bundle exec rails packages:install`

When you download the plugins what it happens is that the information of the plugins will be stored in your database. While the `install` will export this information and will create the AppPackage with the proper files in your codebase.

To find your `CHASKIQ_APPSTORE_KEY` go to the appstore.chaskiq.io site and see the.

Developing and managing Chaskiq plugins is a great way to extend the functionality of your Chaskiq application and provide additional value to your users. By following these guidelines, you can ensure that your plugins are high-quality, reliable, and easy to use. Happy coding!
