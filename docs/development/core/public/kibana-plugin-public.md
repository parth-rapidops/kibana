<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [kibana-plugin-public](./kibana-plugin-public.md)

## kibana-plugin-public package

The Kibana Core APIs for client-side plugins.

A plugin's `public/index` file must contain a named import, `plugin`<!-- -->, that implements [PluginInitializer](./kibana-plugin-public.plugininitializer.md) which returns an object that implements [Plugin](./kibana-plugin-public.plugin.md)<!-- -->.

The plugin integrates with the core system via lifecycle events: `setup`<!-- -->, `start`<!-- -->, and `stop`<!-- -->. In each lifecycle method, the plugin will receive the corresponding core services available (either [CoreSetup](./kibana-plugin-public.coresetup.md) or [CoreStart](./kibana-plugin-public.corestart.md)<!-- -->) and any interfaces returned by dependency plugins' lifecycle method. Anything returned by the plugin's lifecycle method will be exposed to downstream dependencies when their corresponding lifecycle methods are invoked.

## Classes

|  Class | Description |
|  --- | --- |
|  [HttpInterceptController](./kibana-plugin-public.httpinterceptcontroller.md) |  |
|  [SavedObjectsClient](./kibana-plugin-public.savedobjectsclient.md) | Saved Objects is Kibana's data persisentence mechanism allowing plugins to use Elasticsearch for storing plugin state. The client-side SavedObjectsClient is a thin convenience library around the SavedObjects HTTP API for interacting with Saved Objects. |
|  [SimpleSavedObject](./kibana-plugin-public.simplesavedobject.md) | This class is a very simple wrapper for SavedObjects loaded from the server with the [SavedObjectsClient](./kibana-plugin-public.savedobjectsclient.md)<!-- -->.<!-- -->It provides basic functionality for creating/saving/deleting saved objects, but doesn't include any type-specific implementations. |
|  [ToastsApi](./kibana-plugin-public.toastsapi.md) |  |
|  [UiSettingsClient](./kibana-plugin-public.uisettingsclient.md) |  |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [App](./kibana-plugin-public.app.md) | Extension of [common app properties](./kibana-plugin-public.appbase.md) with the mount function. |
|  [AppBase](./kibana-plugin-public.appbase.md) |  |
|  [ApplicationSetup](./kibana-plugin-public.applicationsetup.md) |  |
|  [ApplicationStart](./kibana-plugin-public.applicationstart.md) |  |
|  [AppMountContext](./kibana-plugin-public.appmountcontext.md) | The context object received when applications are mounted to the DOM. |
|  [AppMountParameters](./kibana-plugin-public.appmountparameters.md) |  |
|  [Capabilities](./kibana-plugin-public.capabilities.md) | The read-only set of capabilities available for the current UI session. Capabilities are simple key-value pairs of (string, boolean), where the string denotes the capability ID, and the boolean is a flag indicating if the capability is enabled or disabled. |
|  [ChromeBadge](./kibana-plugin-public.chromebadge.md) |  |
|  [ChromeBrand](./kibana-plugin-public.chromebrand.md) |  |
|  [ChromeBreadcrumb](./kibana-plugin-public.chromebreadcrumb.md) |  |
|  [ChromeNavControl](./kibana-plugin-public.chromenavcontrol.md) |  |
|  [ChromeNavControls](./kibana-plugin-public.chromenavcontrols.md) | [APIs](./kibana-plugin-public.chromenavcontrols.md) for registering new controls to be displayed in the navigation bar. |
|  [ChromeNavLink](./kibana-plugin-public.chromenavlink.md) |  |
|  [ChromeNavLinks](./kibana-plugin-public.chromenavlinks.md) | [APIs](./kibana-plugin-public.chromenavlinks.md) for manipulating nav links. |
|  [ChromeRecentlyAccessed](./kibana-plugin-public.chromerecentlyaccessed.md) | [APIs](./kibana-plugin-public.chromerecentlyaccessed.md) for recently accessed history. |
|  [ChromeRecentlyAccessedHistoryItem](./kibana-plugin-public.chromerecentlyaccessedhistoryitem.md) |  |
|  [ChromeStart](./kibana-plugin-public.chromestart.md) | ChromeStart allows plugins to customize the global chrome header UI and enrich the UX with additional information about the current location of the browser. |
|  [ContextSetup](./kibana-plugin-public.contextsetup.md) | An object that handles registration of context providers and configuring handlers with context. |
|  [CoreSetup](./kibana-plugin-public.coresetup.md) | Core services exposed to the <code>Plugin</code> setup lifecycle |
|  [CoreStart](./kibana-plugin-public.corestart.md) | Core services exposed to the <code>Plugin</code> start lifecycle |
|  [DocLinksStart](./kibana-plugin-public.doclinksstart.md) |  |
|  [ErrorToastOptions](./kibana-plugin-public.errortoastoptions.md) |  |
|  [FatalErrorInfo](./kibana-plugin-public.fatalerrorinfo.md) | Represents the <code>message</code> and <code>stack</code> of a fatal Error |
|  [FatalErrorsSetup](./kibana-plugin-public.fatalerrorssetup.md) | FatalErrors stop the Kibana Public Core and displays a fatal error screen with details about the Kibana build and the error. |
|  [HttpErrorRequest](./kibana-plugin-public.httperrorrequest.md) |  |
|  [HttpErrorResponse](./kibana-plugin-public.httperrorresponse.md) |  |
|  [HttpFetchOptions](./kibana-plugin-public.httpfetchoptions.md) |  |
|  [HttpFetchQuery](./kibana-plugin-public.httpfetchquery.md) |  |
|  [HttpHeadersInit](./kibana-plugin-public.httpheadersinit.md) |  |
|  [HttpInterceptor](./kibana-plugin-public.httpinterceptor.md) |  |
|  [HttpRequestInit](./kibana-plugin-public.httprequestinit.md) |  |
|  [HttpResponse](./kibana-plugin-public.httpresponse.md) |  |
|  [HttpServiceBase](./kibana-plugin-public.httpservicebase.md) |  |
|  [I18nStart](./kibana-plugin-public.i18nstart.md) | I18nStart.Context is required by any localizable React component from @<!-- -->kbn/i18n and @<!-- -->elastic/eui packages and is supposed to be used as the topmost component for any i18n-compatible React tree. |
|  [IContextContainer](./kibana-plugin-public.icontextcontainer.md) | An object that handles registration of context providers and configuring handlers with context. |
|  [LegacyCoreSetup](./kibana-plugin-public.legacycoresetup.md) | Setup interface exposed to the legacy platform via the <code>ui/new_platform</code> module. |
|  [LegacyCoreStart](./kibana-plugin-public.legacycorestart.md) | Start interface exposed to the legacy platform via the <code>ui/new_platform</code> module. |
|  [LegacyNavLink](./kibana-plugin-public.legacynavlink.md) |  |
|  [NotificationsSetup](./kibana-plugin-public.notificationssetup.md) |  |
|  [NotificationsStart](./kibana-plugin-public.notificationsstart.md) |  |
|  [OverlayBannersStart](./kibana-plugin-public.overlaybannersstart.md) |  |
|  [OverlayRef](./kibana-plugin-public.overlayref.md) |  |
|  [OverlayStart](./kibana-plugin-public.overlaystart.md) |  |
|  [Plugin](./kibana-plugin-public.plugin.md) | The interface that should be returned by a <code>PluginInitializer</code>. |
|  [PluginInitializerContext](./kibana-plugin-public.plugininitializercontext.md) | The available core services passed to a <code>PluginInitializer</code> |
|  [SavedObject](./kibana-plugin-public.savedobject.md) |  |
|  [SavedObjectAttributes](./kibana-plugin-public.savedobjectattributes.md) | The data for a Saved Object is stored as an object in the <code>attributes</code> property. |
|  [SavedObjectReference](./kibana-plugin-public.savedobjectreference.md) | A reference to another saved object. |
|  [SavedObjectsBaseOptions](./kibana-plugin-public.savedobjectsbaseoptions.md) |  |
|  [SavedObjectsBatchResponse](./kibana-plugin-public.savedobjectsbatchresponse.md) |  |
|  [SavedObjectsBulkCreateObject](./kibana-plugin-public.savedobjectsbulkcreateobject.md) |  |
|  [SavedObjectsBulkCreateOptions](./kibana-plugin-public.savedobjectsbulkcreateoptions.md) |  |
|  [SavedObjectsCreateOptions](./kibana-plugin-public.savedobjectscreateoptions.md) |  |
|  [SavedObjectsFindOptions](./kibana-plugin-public.savedobjectsfindoptions.md) |  |
|  [SavedObjectsFindResponsePublic](./kibana-plugin-public.savedobjectsfindresponsepublic.md) | Return type of the Saved Objects <code>find()</code> method.<!-- -->\*Note\*: this type is different between the Public and Server Saved Objects clients. |
|  [SavedObjectsMigrationVersion](./kibana-plugin-public.savedobjectsmigrationversion.md) | Information about the migrations that have been applied to this SavedObject. When Kibana starts up, KibanaMigrator detects outdated documents and migrates them based on this value. For each migration that has been applied, the plugin's name is used as a key and the latest migration version as the value. |
|  [SavedObjectsStart](./kibana-plugin-public.savedobjectsstart.md) |  |
|  [SavedObjectsUpdateOptions](./kibana-plugin-public.savedobjectsupdateoptions.md) |  |
|  [UiSettingsState](./kibana-plugin-public.uisettingsstate.md) |  |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [AppUnmount](./kibana-plugin-public.appunmount.md) | A function called when an application should be unmounted from the page. This function should be synchronous. |
|  [ChromeHelpExtension](./kibana-plugin-public.chromehelpextension.md) |  |
|  [ChromeNavLinkUpdateableFields](./kibana-plugin-public.chromenavlinkupdateablefields.md) |  |
|  [HandlerContextType](./kibana-plugin-public.handlercontexttype.md) | Extracts the type of the first argument of a [HandlerFunction](./kibana-plugin-public.handlerfunction.md) to represent the type of the context. |
|  [HandlerFunction](./kibana-plugin-public.handlerfunction.md) | A function that accepts a context object and an optional number of additional arguments. Used for the generic types in [IContextContainer](./kibana-plugin-public.icontextcontainer.md) |
|  [HandlerParameters](./kibana-plugin-public.handlerparameters.md) | Extracts the types of the additional arguments of a [HandlerFunction](./kibana-plugin-public.handlerfunction.md)<!-- -->, excluding the [HandlerContextType](./kibana-plugin-public.handlercontexttype.md)<!-- -->. |
|  [HttpBody](./kibana-plugin-public.httpbody.md) |  |
|  [HttpHandler](./kibana-plugin-public.httphandler.md) |  |
|  [HttpSetup](./kibana-plugin-public.httpsetup.md) |  |
|  [HttpStart](./kibana-plugin-public.httpstart.md) |  |
|  [IContextProvider](./kibana-plugin-public.icontextprovider.md) | A function that returns a context value for a specific key of given context type. |
|  [OverlayBannerMount](./kibana-plugin-public.overlaybannermount.md) | A function that will mount the banner inside the provided element. |
|  [OverlayBannerUnmount](./kibana-plugin-public.overlaybannerunmount.md) | A function that will unmount the banner from the element. |
|  [PluginInitializer](./kibana-plugin-public.plugininitializer.md) | The <code>plugin</code> export at the root of a plugin's <code>public</code> directory should conform to this interface. |
|  [PluginOpaqueId](./kibana-plugin-public.pluginopaqueid.md) |  |
|  [RecursiveReadonly](./kibana-plugin-public.recursivereadonly.md) |  |
|  [SavedObjectAttribute](./kibana-plugin-public.savedobjectattribute.md) | Type definition for a Saved Object attribute value |
|  [SavedObjectAttributeSingle](./kibana-plugin-public.savedobjectattributesingle.md) | Don't use this type, it's simply a helper type for [SavedObjectAttribute](./kibana-plugin-public.savedobjectattribute.md) |
|  [SavedObjectsClientContract](./kibana-plugin-public.savedobjectsclientcontract.md) | SavedObjectsClientContract as implemented by the [SavedObjectsClient](./kibana-plugin-public.savedobjectsclient.md) |
|  [ToastInput](./kibana-plugin-public.toastinput.md) |  |
|  [UiSettingsClientContract](./kibana-plugin-public.uisettingsclientcontract.md) | [UiSettingsClient](./kibana-plugin-public.uisettingsclient.md) |
