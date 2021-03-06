---
title: "Module managementgroups"
title_tag: "Module managementgroups | Package @pulumi/azure | Node.js SDK"
linktitle: "managementgroups"
meta_desc: "Explore members of the managementgroups module in the @pulumi/azure package."
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
    <li><a href="#ManagementGroup"><span class="symbol resource"></span>ManagementGroup</a></li>
</ul>

<h3>Functions</h3>
<ul class="api">
    <li><a href="#getManagementGroup"><span class="symbol function"></span>getManagementGroup</a></li>
</ul>

<h3>Others</h3>
<ul class="api">
    <li><a href="#GetManagementGroupArgs"><span class="symbol api"></span>GetManagementGroupArgs</a></li>
    <li><a href="#GetManagementGroupResult"><span class="symbol api"></span>GetManagementGroupResult</a></li>
    <li><a href="#ManagementGroupArgs"><span class="symbol api"></span>ManagementGroupArgs</a></li>
    <li><a href="#ManagementGroupState"><span class="symbol api"></span>ManagementGroupState</a></li>
</ul>


<h2 id="resources">Resources</h2>
<h3 class="pdoc-module-header" id="ManagementGroup" data-link-title="ManagementGroup">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L32">
        Resource <strong>ManagementGroup</strong>
    </a>
</h3>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
azure.managementgroups.ManagementGroup has been deprecated in favor of azure.management.Group
</div>
<pre class="highlight"><code><span class='kr'>class</span> <span class='nx'>ManagementGroup</span> <span class='kr'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></code></pre>
<h4 class="pdoc-member-header" id="ManagementGroup-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L79"> <b>constructor</b></a>
</h4>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
azure.managementgroups.ManagementGroup has been deprecated in favor of azure.management.Group
</div>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
azure.managementgroups.ManagementGroup has been deprecated in favor of azure.management.Group
</div>
<pre class="highlight"><code><span class='kd'></span><span class='kd'>new</span> ManagementGroup(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: <a href='#ManagementGroupArgs'>ManagementGroupArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</code></pre>

<h4 class="pdoc-member-header" id="ManagementGroup-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L41">method <b>get</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#ManagementGroupState'>ManagementGroupState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#ManagementGroup'>ManagementGroup</a></code></pre>


Get an existing ManagementGroup resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h4 class="pdoc-member-header" id="ManagementGroup-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L32">method <b>getProvider</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ProviderResource'>ProviderResource</a> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></code></pre>

<h4 class="pdoc-member-header" id="ManagementGroup-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L53">method <b>isInstance</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): obj is ManagementGroup</code></pre>


Returns true if the given object is an instance of ManagementGroup.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

<h4 class="pdoc-member-header" id="ManagementGroup-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L63">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>displayName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A friendly name for this Management Group. If not specified, this'll be the same as the `name`.

<h4 class="pdoc-member-header" id="ManagementGroup-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L67">property <b>groupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>groupId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroup-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L32">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</code></pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h4 class="pdoc-member-header" id="ManagementGroup-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L71">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroup-parentManagementGroupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L75">property <b>parentManagementGroupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>parentManagementGroupId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the Parent Management Group. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroup-subscriptionIds">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L79">property <b>subscriptionIds</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>subscriptionIds: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[] | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

A list of Subscription GUIDs which should be assigned to the Management Group.

<h4 class="pdoc-member-header" id="ManagementGroup-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L32">property <b>urn</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</code></pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.


<h2 id="functions">Functions</h2>
<h3 class="pdoc-module-header" id="getManagementGroup" data-link-title="getManagementGroup">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L25">
        Function <strong>getManagementGroup</strong>
    </a>
</h3>


<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
azure.managementgroups.getManagementGroup has been deprecated in favor of azure.management.getGroup
</div>
<pre class="highlight"><code><span class='kd'></span>getManagementGroup(args?: <a href='#GetManagementGroupArgs'>GetManagementGroupArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions'>pulumi.InvokeOptions</a>): <a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise'>Promise</a>&lt;<a href='#GetManagementGroupResult'>GetManagementGroupResult</a>&gt;</code></pre>


<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="GetManagementGroupArgs" data-link-title="GetManagementGroupArgs">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L44">
        interface <strong>GetManagementGroupArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetManagementGroupArgs</span></code></pre>

A collection of arguments for invoking getManagementGroup.

<h4 class="pdoc-member-header" id="GetManagementGroupArgs-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L49">property <b>groupId</b></a>
</h4>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
Deprecated in favour of `name`
</div>
<pre class="highlight"><code><span class='kd'></span>groupId?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

Specifies the name or UUID of this Management Group.

<h4 class="pdoc-member-header" id="GetManagementGroupArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L53">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

Specifies the name or UUID of this Management Group.

<h3 class="pdoc-module-header" id="GetManagementGroupResult" data-link-title="GetManagementGroupResult">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L59">
        interface <strong>GetManagementGroupResult</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>GetManagementGroupResult</span></code></pre>

A collection of values returned by getManagementGroup.

<h4 class="pdoc-member-header" id="GetManagementGroupResult-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L63">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>displayName: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

A friendly name for the Management Group.

<h4 class="pdoc-member-header" id="GetManagementGroupResult-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L64">property <b>groupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>groupId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>
<h4 class="pdoc-member-header" id="GetManagementGroupResult-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L77">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The provider-assigned unique ID for this managed resource.

<h4 class="pdoc-member-header" id="GetManagementGroupResult-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L65">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>
<h4 class="pdoc-member-header" id="GetManagementGroupResult-parentManagementGroupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L69">property <b>parentManagementGroupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>parentManagementGroupId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;</code></pre>

The ID of any Parent Management Group.

<h4 class="pdoc-member-header" id="GetManagementGroupResult-subscriptionIds">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/getManagementGroup.ts#L73">property <b>subscriptionIds</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>subscriptionIds: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];</code></pre>

A list of Subscription ID's which are assigned to the Management Group.

<h3 class="pdoc-module-header" id="ManagementGroupArgs" data-link-title="ManagementGroupArgs">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L150">
        interface <strong>ManagementGroupArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ManagementGroupArgs</span></code></pre>

The set of arguments for constructing a ManagementGroup resource.

<h4 class="pdoc-member-header" id="ManagementGroupArgs-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L154">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A friendly name for this Management Group. If not specified, this'll be the same as the `name`.

<h4 class="pdoc-member-header" id="ManagementGroupArgs-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L159">property <b>groupId</b></a>
</h4>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
Deprecated in favour of `name`
</div>
<pre class="highlight"><code><span class='kd'></span>groupId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L163">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupArgs-parentManagementGroupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L167">property <b>parentManagementGroupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>parentManagementGroupId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the Parent Management Group. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupArgs-subscriptionIds">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L171">property <b>subscriptionIds</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>subscriptionIds?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>

A list of Subscription GUIDs which should be assigned to the Management Group.

<h3 class="pdoc-module-header" id="ManagementGroupState" data-link-title="ManagementGroupState">
    <a href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L123">
        interface <strong>ManagementGroupState</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>ManagementGroupState</span></code></pre>

Input properties used for looking up and filtering ManagementGroup resources.

<h4 class="pdoc-member-header" id="ManagementGroupState-displayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L127">property <b>displayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>displayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

A friendly name for this Management Group. If not specified, this'll be the same as the `name`.

<h4 class="pdoc-member-header" id="ManagementGroupState-groupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L132">property <b>groupId</b></a>
</h4>

<div class="note note-deprecated">
<i class="fas fa-exclamation-triangle pr-2"></i><strong>DEPRECATED</strong>
Deprecated in favour of `name`
</div>
<pre class="highlight"><code><span class='kd'></span>groupId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L136">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The name or UUID for this Management Group, which needs to be unique across your tenant. A new UUID will be generated if not provided. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupState-parentManagementGroupId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L140">property <b>parentManagementGroupId</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>parentManagementGroupId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The ID of the Parent Management Group. Changing this forces a new resource to be created.

<h4 class="pdoc-member-header" id="ManagementGroupState-subscriptionIds">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-azure/blob/4f564ccfe63bf4827fa00f82d904d97b6b38ceb3/sdk/nodejs/managementgroups/managementGroup.ts#L144">property <b>subscriptionIds</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>subscriptionIds?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>

A list of Subscription GUIDs which should be assigned to the Management Group.

