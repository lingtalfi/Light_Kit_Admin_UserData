Light_Kit_Admin_UserData
===========
2020-02-28 -> 2020-08-07



This plugin hooks the [Light_UserData](https://github.com/lingtalfi/Light_UserData) plugin into the [Light_Kit_Admin](https://github.com/lingtalfi/Light_Kit_Admin) environment.


This is a [Light plugin](https://github.com/lingtalfi/Light/blob/master/doc/pages/plugin.md).

This is part of the [universe framework](https://github.com/karayabin/universe-snapshot).


Install
==========
Using the [uni](https://github.com/lingtalfi/universe-naive-importer) command.
```bash
uni import Ling/Light_Kit_Admin_UserData
```

Or just download it and place it where you want otherwise.






Summary
===========
- [Light_Kit_Admin_UserData api](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/doc/api/Ling/Light_Kit_Admin_UserData.md) (generated with [DocTools](https://github.com/lingtalfi/DocTools))
- Pages
    - [Conception notes](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/doc/pages/conception-notes.md)
- [Services](#services)



Services
=========


This plugin provides the following services:

- kit_admin_user_data (returns a LightKitAdminUserDataService instance)


Here is an example of the service configuration:

```yaml
user_data:
    instance: Ling\Light_UserData\Service\LightUserDataService
    methods:
        setContainer:
            container: @container()
        setObfuscationParams:
            algo: default
            secret: P0zeg7e,4dD
        setRootDir:
            dir: ${app_dir}/user-data



# --------------------------------------
# hooks
# --------------------------------------
$ajax_handler.methods_collection:
    -
        method: registerHandler
        args:
            id: Light_UserData
            handler:
                instance: Ling\Light_UserData\AjaxHandler\LightUserDataAjaxHandler


$breeze_generator.methods_collection:
    -
        method: addConfigurationEntryByFile
        args:
            key: luda
            file: ${app_dir}/config/data/Light_UserData/Light_BreezeGenerator/luda.byml


$easy_route.methods_collection:
    -
        method: registerBundleFile
        args:
            file: config/data/Light_UserData/Light_EasyRoute/luda_routes.byml


$events.methods_collection:
    -
        method: registerListener
        args:
            events: Light_Database.on_lud_user_group_create
            listener:
                instance: @service(user_data)
                callable_method: onUserGroupCreate


$plugin_installer.methods_collection:
    -
        method: registerPlugin
        args:
            plugin: Light_UserData
            installer: @service(user_data)





```



History Log
=============

- 1.5.0 -- 2020-08-07

    - update service to adapt realform late registration
    
- 1.4.0 -- 2020-08-07

    - update service to adapt realist late registration
    
- 1.3.0 -- 2020-06-23

    - update service to adapt new plugin installer service

- 1.2.0 -- 2020-03-06

    - update kit admin generator config: use a shortName variable to make it more compact
    
- 1.1.0 -- 2020-03-05

    - change kit admin generator config to take into account user row restriction
    
- 1.0.0 -- 2020-02-28

    - initial commit