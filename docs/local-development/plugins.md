## Local development

Chaskiq will have some built in plugins if you want to download the chaskiq catalog you will need the CHASKIQ_APPSTORE_KEY, in order to get the plugins run this command:


`rails packages:download`

The command above will download the plungin information and will store that in the `plugins` table, those record will have a corresponding AppPackage association.

In order to get the plugin files installed on your Chaskiq instance run the following command:

`rails packages:install`

The command above will load the data from the `Plugin` and save those in the filesystem on app/services/message_apis/{PLUGIN}

If you are developing a local plugin that exists on the catalog then your plugin could be overriden by the installation. In order to avoid that you can froze a plugin by doing:

`bundle exec rails packages:unfreeze['Zapier']`

the command above will mark the app package as frozen and then it will only use your local copy of the plugin wihout modifying the plugin files on the `packages:download` or `packages:install` commands.
