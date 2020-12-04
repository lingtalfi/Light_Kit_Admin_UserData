[Back to the Ling/Light_Kit_Admin_UserData api](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/doc/api/Ling/Light_Kit_Admin_UserData.md)



The LkaUserDataFileManagerWidget class
================
2020-02-28 --> 2020-12-04






Introduction
============

The LkaUserDataFileManagerWidget class.



Class synopsis
==============


class <span class="pl-k">LkaUserDataFileManagerWidget</span> extends EasyLightPicassoWidget implements KitPageRendererAwareInterface, UniversalTemplateEngineInterface, WidgetConfAwarePicassoWidgetInterface {

- Inherited properties
    - protected Ling\Kit\PageRenderer\KitPageRendererInterface [EasyLightPicassoWidget::$kitPageRenderer](#property-kitPageRenderer) ;
    - protected array [WidgetConfAwarePicassoWidget::$widgetConf](#property-widgetConf) ;
    - protected array [PicassoWidget::$libraries](#property-libraries) ;
    - protected array [PicassoWidget::$attr](#property-attr) ;
    - protected Ling\HtmlPageTools\Copilot\HtmlPageCopilot [PicassoWidget::$copilot](#property-copilot) ;

- Inherited methods
    - public EasyLightPicassoWidget::__construct() : void
    - public EasyLightPicassoWidget::setKitPageRenderer(Ling\Kit\PageRenderer\KitPageRendererInterface $renderer) : void
    - public EasyLightPicassoWidget::getKitPageRenderer() : Ling\Kit\PageRenderer\KitPageRendererInterface | null
    - protected EasyLightPicassoWidget::getContainer() : [LightServiceContainerInterface](https://github.com/lingtalfi/Light/blob/master/doc/api/Ling/Light/ServiceContainer/LightServiceContainerInterface.md)
    - public WidgetConfAwarePicassoWidget::setWidgetConf(array $widgetConf) : void
    - public WidgetConfAwarePicassoWidget::getWidgetConf() : array
    - public PicassoWidget::getLibraries() : array
    - public PicassoWidget::setCopilot(Ling\HtmlPageTools\Copilot\HtmlPageCopilot $copilot) : void
    - public PicassoWidget::renderFile(string $filePath, ?array $variables = []) : false | string
    - public PicassoWidget::prepare(array &$widgetConf, Ling\HtmlPageTools\Copilot\HtmlPageCopilot $copilot) : void
    - protected PicassoWidget::getAttributesHtml(?bool $excludeClass = true) : string
    - protected PicassoWidget::getCssClass() : string
    - protected PicassoWidget::registerLibrary(string $libraryName, array $css, array $js) : void
    - public ZephyrTemplateEngine::render(string $resourceId, ?array $variables = []) : false | string
    - public ZephyrTemplateEngine::getErrors() : array
    - public ZephyrTemplateEngine::setDirectory(string $directory) : void
    - protected ZephyrTemplateEngine::interpret(string $___path, array $z) : false | string
    - private ZephyrTemplateEngine::addError(string $msg) : void

}






Methods
==============

- EasyLightPicassoWidget::__construct &ndash; Builds the EasyPicassoWidget instance.
- EasyLightPicassoWidget::setKitPageRenderer &ndash; Sets the KitPageRenderer instance.
- EasyLightPicassoWidget::getKitPageRenderer &ndash; 
- EasyLightPicassoWidget::getContainer &ndash; Returns a light service container instance.
- WidgetConfAwarePicassoWidget::setWidgetConf &ndash; Sets the widget configuration.
- WidgetConfAwarePicassoWidget::getWidgetConf &ndash; Returns the widget configuration.
- PicassoWidget::getLibraries &ndash; Returns the libraries of this instance.
- PicassoWidget::setCopilot &ndash; Sets the copilot.
- PicassoWidget::renderFile &ndash; Parses the file identified and returns its interpreted content (by injecting the variables in it).
- PicassoWidget::prepare &ndash; Prepares the widget according to the given widget configuration.
- PicassoWidget::getAttributesHtml &ndash; Returns the string of html attributes defined in the widget attributes (attr property in the widget configuration array).
- PicassoWidget::getCssClass &ndash; 
- PicassoWidget::registerLibrary &ndash; Registers an (external) library that this widget uses.
- ZephyrTemplateEngine::render &ndash; Parses the template identified by $resourceId and returns the interpreted template (the template with the variables injected in it).
- ZephyrTemplateEngine::getErrors &ndash; Returns the errors of this instance.
- ZephyrTemplateEngine::setDirectory &ndash; Sets the directory.
- ZephyrTemplateEngine::interpret &ndash; and returns the resulting html code.
- ZephyrTemplateEngine::addError &ndash; Adds an error to this instance.





Location
=============
Ling\Light_Kit_Admin_UserData\Light_Kit\Widget\Picasso\LkaUserDataFileManagerWidget<br>
See the source code of [Ling\Light_Kit_Admin_UserData\Light_Kit\Widget\Picasso\LkaUserDataFileManagerWidget](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/Light_Kit/Widget/Picasso/LkaUserDataFileManagerWidget.php)



SeeAlso
==============
Previous class: [LightKitAdminUserDataControllerHubHandler](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/doc/api/Ling/Light_Kit_Admin_UserData/Light_ControllerHub/Generated/LightKitAdminUserDataControllerHubHandler.md)<br>Next class: [LightKitAdminUserDataDuplicator](https://github.com/lingtalfi/Light_Kit_Admin_UserData/blob/master/doc/api/Ling/Light_Kit_Admin_UserData/Light_Kit_Admin/Duplicator/LightKitAdminUserDataDuplicator.md)<br>