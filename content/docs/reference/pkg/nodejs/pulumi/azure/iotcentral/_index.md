---
title: "Module iotcentral"
title_tag: "Module iotcentral | Package @pulumi/azure | Node.js SDK"
linktitle: "iotcentral"
meta_desc: "Explore members of the iotcentral module in the @pulumi/azure package."
git_sha: "4f564ccfe63bf4827fa00f82d904d97b6b38ceb3"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-azurerm)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-azure` repo](https://github.com/pulumi/pulumi-azure/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-azurerm` repo](https://github.com/terraform-providers/terraform-provider-azurerm/issues).





<h3>Resources</h3>
<ul class="api">
    <li><a href="#Application"><span class="symbol resource"></span>Application</a></li>
</ul>


<h3>Others</h3>
<ul class="api">
    <li><a href="#ApplicationArgs"><span class="symbol api"></span>ApplicationArgs</a></li>
    <li><a href="#ApplicationState"><span class="symbol api"></span>ApplicationState</a></li>
</ul>


<h2 id="resources">Resources</h2>
<h3 class="pdoc-module-header" id="Application" data-link-title="Application">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L32">
        Resource <strong>Application</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>class</span> <span class='nx'>Application</span> <span class='kr'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></code></pre>

Manages an IoT Central Application

#### Example Usage



```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure from "@pulumi/azure";

const exampleResourceGroup = new azure.core.ResourceGroup("exampleResourceGroup", {location: "West Europe"});
const exampleApplication = new azure.iotcentral.Application("exampleApplication", {
    resourceGroupName: exampleResourceGroup.name,
    location: exampleResourceGroup.location,
    subDomain: "example-iotcentral-app-subdomain",
    displayName: "example-iotcentral-app-display-name",
    sku: "S1",
    template: "iotc-default@1.0.0",
    tags: {
        Foo: "Bar",
    },
});
```

<h4 class="pdoc-member-header" id="Application-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L90"> <b>constructor</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span><span class='kd'>new</span> Application(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#ApplicationArgs'>ApplicationArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</code></pre>


Create a Application resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h4 class="pdoc-member-header" id="Application-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L41">method <b>get</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#ApplicationState'>ApplicationState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Application'>Application</a></code></pre>


Get an existing Application resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h4 class="pdoc-member-header" id="Application-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L32">method <b>getProvider</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ProviderResource'>ProviderResource</a> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></code></pre>

<h4 class="pdoc-member-header" id="Application-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L52">method <b>isInstance</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): obj is Application</code></pre>


Returns true if the given object is an instance of Application.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

<h4 class="pdoc-member-header" id="Application-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L62">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>displayName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `displayName` name. Custom display name for the IoT Central application. Default is resource name.

<h4 class="pdoc-member-header" id="Application-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L32">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</code></pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h4 class="pdoc-member-header" id="Application-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L66">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>location: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the supported Azure location where the resource has to be create. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="Application-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L70">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the name of the IotHub resource. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="Application-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L74">property <b>resourceGroupName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>resourceGroupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name of the resource group under which the IotHub resource has to be created. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="Application-sku">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L78">property <b>sku</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>sku: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

A `sku` name. Possible values is `ST1`, `ST2`, Default value is `ST1`

<h4 class="pdoc-member-header" id="Application-subDomain">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L82">property <b>subDomain</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>subDomain: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `subDomain` name. Subdomain for the IoT Central URL. Each application must have a unique subdomain.

<h4 class="pdoc-member-header" id="Application-tags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L86">property <b>tags</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>tags: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

A mapping of tags to assign to the resource.

<h4 class="pdoc-member-header" id="Application-template">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L90">property <b>template</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>template: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `template` name. IoT Central application template name. Default is a custom application.

<h4 class="pdoc-member-header" id="Application-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L32">property <b>urn</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</code></pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.



<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="ApplicationArgs" data-link-title="ApplicationArgs">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L181">
        interface <strong>ApplicationArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ApplicationArgs</span></code></pre>

The set of arguments for constructing a Application resource.

<h4 class="pdoc-member-header" id="ApplicationArgs-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L185">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `displayName` name. Custom display name for the IoT Central application. Default is resource name.

<h4 class="pdoc-member-header" id="ApplicationArgs-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L189">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>location?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the supported Azure location where the resource has to be create. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L193">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the name of the IotHub resource. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationArgs-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L197">property <b>resourceGroupName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>resourceGroupName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name of the resource group under which the IotHub resource has to be created. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationArgs-sku">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L201">property <b>sku</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>sku?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `sku` name. Possible values is `ST1`, `ST2`, Default value is `ST1`

<h4 class="pdoc-member-header" id="ApplicationArgs-subDomain">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L205">property <b>subDomain</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>subDomain: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `subDomain` name. Subdomain for the IoT Central URL. Each application must have a unique subdomain.

<h4 class="pdoc-member-header" id="ApplicationArgs-tags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L209">property <b>tags</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>tags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</code></pre>

A mapping of tags to assign to the resource.

<h4 class="pdoc-member-header" id="ApplicationArgs-template">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L213">property <b>template</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>template?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `template` name. IoT Central application template name. Default is a custom application.

<h3 class="pdoc-module-header" id="ApplicationState" data-link-title="ApplicationState">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L143">
        interface <strong>ApplicationState</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ApplicationState</span></code></pre>

Input properties used for looking up and filtering Application resources.

<h4 class="pdoc-member-header" id="ApplicationState-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L147">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `displayName` name. Custom display name for the IoT Central application. Default is resource name.

<h4 class="pdoc-member-header" id="ApplicationState-location">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L151">property <b>location</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>location?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the supported Azure location where the resource has to be create. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L155">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Specifies the name of the IotHub resource. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationState-resourceGroupName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L159">property <b>resourceGroupName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>resourceGroupName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name of the resource group under which the IotHub resource has to be created. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ApplicationState-sku">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L163">property <b>sku</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>sku?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `sku` name. Possible values is `ST1`, `ST2`, Default value is `ST1`

<h4 class="pdoc-member-header" id="ApplicationState-subDomain">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L167">property <b>subDomain</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>subDomain?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `subDomain` name. Subdomain for the IoT Central URL. Each application must have a unique subdomain.

<h4 class="pdoc-member-header" id="ApplicationState-tags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L171">property <b>tags</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>tags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</code></pre>

A mapping of tags to assign to the resource.

<h4 class="pdoc-member-header" id="ApplicationState-template">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/iotcentral/application.ts#L175">property <b>template</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>template?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A `template` name. IoT Central application template name. Default is a custom application.

