## Chaskiq AppStore Integration

To synchronize the plugins of the Chaskiq AppStore, you need to download them using your `license_key`.

1.  Add your `CHASKIQ_APPSTORE_KEY` to your environment variables. If you're in development mode, include it in the `.env` file.
2.  Execute the `attach` command to download and store the plugins in your database.

`bundle exec rails packages:attach`

**For Chaskiq versions <= 1.2, follow these steps:**

1.  Run the `download` command to download your plugins: `bundle exec rails packages:download`.
2.  Install the downloaded plugins by running: `bundle exec rails packages:install`.

When you download the plugins, their information is stored in your database. The `install` command exports this information and creates the AppPackage with the appropriate files in your codebase.

To get your `CHASKIQ_APPSTORE_KEY`, visit the [appstore.chaskiq.io](https://appstore.chaskiq.io/) website.

Developing and managing Chaskiq plugins is an excellent way to extend your Chaskiq application's functionality and offer additional value to your users. By following these guidelines, you can ensure your plugins are high-quality, reliable, and user-friendly. Happy coding!
