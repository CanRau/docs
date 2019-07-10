---
title: Module athena
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/aws</a> &gt; athena

> This provider is a derived work of the [Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws)
> distributed under [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/). If you encounter a bug or missing feature,
> first check the [`pulumi/pulumi-aws` repo](https://github.com/pulumi/pulumi-aws/issues); however, if that doesn't turn up anything,
> please consult the source [`terraform-providers/terraform-provider-aws` repo](https://github.com/terraform-providers/terraform-provider-aws/issues).



<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Database">class Database</a></li>
<li><a href="#NamedQuery">class NamedQuery</a></li>
<li><a href="#DatabaseArgs">interface DatabaseArgs</a></li>
<li><a href="#DatabaseState">interface DatabaseState</a></li>
<li><a href="#NamedQueryArgs">interface NamedQueryArgs</a></li>
<li><a href="#NamedQueryState">interface NamedQueryState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts">athena/database.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts">athena/namedQuery.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Database">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L25">class <b>Database</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

Provides an Athena database.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const hogeBucket = new aws.s3.Bucket("hoge", {});
const hogeDatabase = new aws.athena.Database("hoge", {
    bucket: hogeBucket.bucket,
    name: "database_name",
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/athena_database.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="Database-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L67"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Database(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#DatabaseArgs'>DatabaseArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Database resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L34">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#DatabaseState'>DatabaseState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Database'>Database</a></pre>


Get an existing Database resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L45">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Database.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-bucket">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L55">property <b>bucket</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>bucket: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of s3 bucket to save the results of the query execution.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-encryptionConfiguration">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L59">property <b>encryptionConfiguration</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>encryptionConfiguration: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    encryptionOption: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    kmsKey: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

The encryption key block AWS Athena uses to decrypt the data in S3, such as an AWS Key Management Service (AWS KMS) key. An `encryption_configuration` block is documented below.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-forceDestroy">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L63">property <b>forceDestroy</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>forceDestroy: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

A boolean that indicates all tables should be deleted from the database so that the database can be destroyed without error. The tables are *not* recoverable.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L187">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L67">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of the database to create.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Database-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="NamedQuery">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L29">class <b>NamedQuery</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

Provides an Athena Named Query resource.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const hogeBucket = new aws.s3.Bucket("hoge", {});
const hogeDatabase = new aws.athena.Database("hoge", {
    bucket: hogeBucket.bucket,
    name: "users",
});
const foo = new aws.athena.NamedQuery("foo", {
    database: hogeDatabase.name,
    query: pulumi.interpolate`SELECT * FROM ${hogeDatabase.name} limit 10;`,
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/athena_named_query.html.markdown.

{{% /md %}}
<h3 class="pdoc-member-header" id="NamedQuery-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L71"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> NamedQuery(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#NamedQueryArgs'>NamedQueryArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a NamedQuery resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L38">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#NamedQueryState'>NamedQueryState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#NamedQuery'>NamedQuery</a></pre>


Get an existing NamedQuery resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L49">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of NamedQuery.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-database">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L59">property <b>database</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>database: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The database to which the query belongs.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L63">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>description: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

A brief explanation of the query. Maximum length of 1024.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L187">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L67">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The plain language name for the query. Maximum length of 128.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-query">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L71">property <b>query</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>query: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The text of the query itself. In other words, all query statements. Maximum length of 262144.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQuery-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="DatabaseArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L124">interface <b>DatabaseArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Database resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="DatabaseArgs-bucket">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L128">property <b>bucket</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>bucket: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of s3 bucket to save the results of the query execution.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseArgs-encryptionConfiguration">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L132">property <b>encryptionConfiguration</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>encryptionConfiguration?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    encryptionOption: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    kmsKey: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
}&gt;;</pre>
{{% md %}}

The encryption key block AWS Athena uses to decrypt the data in S3, such as an AWS Key Management Service (AWS KMS) key. An `encryption_configuration` block is documented below.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseArgs-forceDestroy">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L136">property <b>forceDestroy</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>forceDestroy?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</pre>
{{% md %}}

A boolean that indicates all tables should be deleted from the database so that the database can be destroyed without error. The tables are *not* recoverable.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L140">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of the database to create.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="DatabaseState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L102">interface <b>DatabaseState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Database resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="DatabaseState-bucket">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L106">property <b>bucket</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>bucket?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of s3 bucket to save the results of the query execution.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseState-encryptionConfiguration">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L110">property <b>encryptionConfiguration</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>encryptionConfiguration?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    encryptionOption: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    kmsKey: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
}&gt;;</pre>
{{% md %}}

The encryption key block AWS Athena uses to decrypt the data in S3, such as an AWS Key Management Service (AWS KMS) key. An `encryption_configuration` block is documented below.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseState-forceDestroy">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L114">property <b>forceDestroy</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>forceDestroy?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</pre>
{{% md %}}

A boolean that indicates all tables should be deleted from the database so that the database can be destroyed without error. The tables are *not* recoverable.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="DatabaseState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/database.ts#L118">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Name of the database to create.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="NamedQueryArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L131">interface <b>NamedQueryArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a NamedQuery resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="NamedQueryArgs-database">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L135">property <b>database</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>database: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The database to which the query belongs.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryArgs-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L139">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A brief explanation of the query. Maximum length of 1024.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L143">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The plain language name for the query. Maximum length of 128.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryArgs-query">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L147">property <b>query</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>query: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The text of the query itself. In other words, all query statements. Maximum length of 262144.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="NamedQueryState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L109">interface <b>NamedQueryState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering NamedQuery resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="NamedQueryState-database">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L113">property <b>database</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>database?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The database to which the query belongs.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryState-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L117">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>description?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

A brief explanation of the query. Maximum length of 1024.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L121">property <b>name</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The plain language name for the query. Maximum length of 128.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="NamedQueryState-query">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/35faf389944ec00da164b2681656a982bf699412/sdk/nodejs/athena/namedQuery.ts#L125">property <b>query</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>query?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

The text of the query itself. In other words, all query statements. Maximum length of 262144.

{{% /md %}}
</div>
</div>