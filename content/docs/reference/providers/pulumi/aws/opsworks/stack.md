---
title: "Stack"
---

<!-- WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

<style>
  table td p { margin-top: 0; margin-bottom: 0; }
</style>

Provides an OpsWorks stack resource.

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/opsworks_stack.html.markdown.


## Create a Stack Resource

{{< langchoose csharp >}}

<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new</span> <span class="nx"><a href=/docs/reference/pkg/nodejs/pulumi/aws/s3/#Stack>Stack</a></span><span class="p">(</span><span class="nx">name</span>: <span class="kt"><a href=https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String>string</a></span><span class="p">,</span> <span class="nx">args</span>: <span class="kt"><a href=/docs/reference/pkg/nodejs/pulumi/aws/s3/#StackArgs>StackArgs</a></span><span class="p">,</span> <span class="nx">opts?</span>: <span class="kt"><a href=/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions>pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>

```python
def __init__(__self__, resource_name, opts=None, agent_version=None, berkshelf_version=None, color=None, configuration_manager_name=None, configuration_manager_version=None, custom_cookbooks_sources=None, custom_json=None, default_availability_zone=None, default_instance_profile_arn=None, default_os=None, default_root_device_type=None, default_ssh_key_name=None, default_subnet_id=None, hostname_theme=None, manage_berkshelf=None, name=None, region=None, service_role_arn=None, tags=None, use_custom_cookbooks=None, use_opsworks_security_groups=None, vpc_id=None, __props__=None)
```

```go
func NewStack(ctx *pulumi.Context, name string, args *StackArgs, opts ...pulumi.ResourceOption) (*Stack, error)

```

```csharp
public Stack(string name, StackArgs args, CustomResourceOptions? options = null)

```

Creates a Stack resource with the given unique name, arguments, and options.

{{% lang nodejs %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>args</strong> &ndash; (Required) The arguments to use to populate this resource's properties.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

{{% lang go %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>args</strong> &ndash; (Required) The arguments to use to populate this resource's properties.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

{{% lang csharp %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>args</strong> &ndash; (Required) The arguments to use to populate this resource's properties.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

The following arguments are supported:

<table class="ml-6">
    <thead>
        <tr>
            <th>Argument</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="align-top">agent<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) If set to `"LATEST"`, OpsWorks will automatically install the latest version.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">berkshelf<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) If `manage_berkshelf` is enabled, the version of Berkshelf to use.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">color</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Color to paint next to the stack's resources in the OpsWorks console.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the configuration manager to use. Defaults to "Chef".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Version of the configuration manager to use. Defaults to "11.4".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Cookbooks<wbr>Sources</td>
            <td class="align-top"><code>Array&lt;<wbr><a href="#stackcustomcookbookssource">Stack<wbr>Custom<wbr>Cookbooks<wbr>Source</a><wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
(Optional) When `use_custom_cookbooks` is set, provide this sub-object as
described below.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Json</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Custom JSON attributes to apply to the entire stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Availability<wbr>Zone</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the availability zone where instances will be created
by default. This is required unless you set `vpc_id`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Instance<wbr>Profile<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) The ARN of an IAM Instance Profile that created instances
will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Os</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of OS that will be installed on instances by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Root<wbr>Device<wbr>Type</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the type of root device instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Ssh<wbr>Key<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the SSH keypair that instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Subnet<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Id of the subnet in which instances will be created by default. Mandatory
if `vpc_id` is set, and forbidden if it isn't.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">hostname<wbr>Theme</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Keyword representing the naming scheme that will be used for instance hostnames
within this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">manage<wbr>Berkshelf</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether Opsworks will run Berkshelf for this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The name of the stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">region</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) The name of the region where the stack will exist.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">service<wbr>Role<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) The ARN of an IAM role that the OpsWorks service will act as.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">tags</td>
            <td class="align-top"><code>Map&lt;<wbr>any<wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
(Optional) A mapping of tags to assign to the resource.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Custom<wbr>Cookbooks</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether the custom cookbook settings are
enabled.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Opsworks<wbr>Security<wbr>Groups</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether the standard OpsWorks
security groups apply to created instances.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vpc<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The id of the VPC that this stack belongs to.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## Stack Output Properties

The following output properties are available:

<table class="ml-6">
    <thead>
        <tr>
            <th>Argument</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="align-top">agent<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
If set to `"LATEST"`, OpsWorks will automatically install the latest version.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">berkshelf<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
If `manage_berkshelf` is enabled, the version of Berkshelf to use.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">color</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Color to paint next to the stack's resources in the OpsWorks console.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Name of the configuration manager to use. Defaults to "Chef".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Version of the configuration manager to use. Defaults to "11.4".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Cookbooks<wbr>Sources</td>
            <td class="align-top"><code>Array&lt;<wbr><a href="#stackcustomcookbookssource">Stack<wbr>Custom<wbr>Cookbooks<wbr>Source</a><wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
When `use_custom_cookbooks` is set, provide this sub-object as
described below.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Json</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Custom JSON attributes to apply to the entire stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Availability<wbr>Zone</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Name of the availability zone where instances will be created
by default. This is required unless you set `vpc_id`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Instance<wbr>Profile<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The ARN of an IAM Instance Profile that created instances
will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Os</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Name of OS that will be installed on instances by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Root<wbr>Device<wbr>Type</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Name of the type of root device instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Ssh<wbr>Key<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Name of the SSH keypair that instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Subnet<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Id of the subnet in which instances will be created by default. Mandatory
if `vpc_id` is set, and forbidden if it isn't.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">hostname<wbr>Theme</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
Keyword representing the naming scheme that will be used for instance hostnames
within this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">manage<wbr>Berkshelf</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
Boolean value controlling whether Opsworks will run Berkshelf for this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The name of the stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">region</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The name of the region where the stack will exist.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">service<wbr>Role<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The ARN of an IAM role that the OpsWorks service will act as.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">stack<wbr>Endpoint</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">tags</td>
            <td class="align-top"><code>Map&lt;<wbr>any<wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
A mapping of tags to assign to the resource.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Custom<wbr>Cookbooks</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
Boolean value controlling whether the custom cookbook settings are
enabled.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Opsworks<wbr>Security<wbr>Groups</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
Boolean value controlling whether the standard OpsWorks
security groups apply to created instances.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vpc<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The id of the VPC that this stack belongs to.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## Look up an Existing Stack Resource

{{< langchoose csharp >}}

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: StackState, opts?: pulumi.CustomResourceOptions): Stack;
```

```python
def get(resource_name, id, opts=None, acceleration_status=None, acl=None, arn=None, bucket=None, bucket_domain_name=None, bucket_prefix=None, bucket_regional_domain_name=None, cors_rules=None, force_destroy=None, hosted_zone_id=None, lifecycle_rules=None, loggings=None, object_lock_configuration=None, policy=None, region=None, replication_configuration=None, request_payer=None, server_side_encryption_configuration=None, tags=None, versioning=None, website=None, website_domain=None, website_endpoint=None)
```

```go
func GetBucket(ctx *pulumi.Context, name string, id pulumi.IDInput, state *BucketState, opts ...pulumi.ResourceOption) (*Bucket, error)
```

```csharp
public static Bucket Get(string name, Input<string> id, BucketState? state = null, CustomResourceOptions? options = null);
```

Get an existing Stack resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% lang nodejs %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>id</strong> &ndash; (Required) The _unique_ provider ID of the resource to lookup.</li>
    <li><strong>state</strong> &ndash; (Optional) Any extra arguments used during the lookup.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

{{% lang go %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>id</strong> &ndash; (Required) The _unique_ provider ID of the resource to lookup.</li>
    <li><strong>state</strong> &ndash; (Optional) Any extra arguments used during the lookup.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

{{% lang csharp %}}
<ul class="pl-10">
    <li><strong>name</strong> &ndash; (Required) The unique name of the resulting resource.</li>
    <li><strong>id</strong> &ndash; (Required) The _unique_ provider ID of the resource to lookup.</li>
    <li><strong>state</strong> &ndash; (Optional) Any extra arguments used during the lookup.</li>
    <li><strong>opts</strong> &ndash; (Optional) A bag of options that control this resource's behavior.</li>
</ul>
{{% /lang %}}

The following state arguments are supported:

<table class="ml-6">
    <thead>
        <tr>
            <th>Argument</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="align-top">agent<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) If set to `"LATEST"`, OpsWorks will automatically install the latest version.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">berkshelf<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) If `manage_berkshelf` is enabled, the version of Berkshelf to use.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">color</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Color to paint next to the stack's resources in the OpsWorks console.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the configuration manager to use. Defaults to "Chef".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">configuration<wbr>Manager<wbr>Version</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Version of the configuration manager to use. Defaults to "11.4".

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Cookbooks<wbr>Sources</td>
            <td class="align-top"><code>Array&lt;<wbr><a href="#stackcustomcookbookssource">Stack<wbr>Custom<wbr>Cookbooks<wbr>Source</a><wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
(Optional) When `use_custom_cookbooks` is set, provide this sub-object as
described below.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">custom<wbr>Json</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Custom JSON attributes to apply to the entire stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Availability<wbr>Zone</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the availability zone where instances will be created
by default. This is required unless you set `vpc_id`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Instance<wbr>Profile<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The ARN of an IAM Instance Profile that created instances
will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Os</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of OS that will be installed on instances by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Root<wbr>Device<wbr>Type</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the type of root device instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Ssh<wbr>Key<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Name of the SSH keypair that instances will have by default.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">default<wbr>Subnet<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Id of the subnet in which instances will be created by default. Mandatory
if `vpc_id` is set, and forbidden if it isn't.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">hostname<wbr>Theme</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) Keyword representing the naming scheme that will be used for instance hostnames
within this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">manage<wbr>Berkshelf</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether Opsworks will run Berkshelf for this stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The name of the stack.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">region</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The name of the region where the stack will exist.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">service<wbr>Role<wbr>Arn</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The ARN of an IAM role that the OpsWorks service will act as.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">stack<wbr>Endpoint</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">tags</td>
            <td class="align-top"><code>Map&lt;<wbr>any<wbr>&gt;</code></td>
            <td class="align-top">{{% md %}}
(Optional) A mapping of tags to assign to the resource.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Custom<wbr>Cookbooks</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether the custom cookbook settings are
enabled.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">use<wbr>Opsworks<wbr>Security<wbr>Groups</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean value controlling whether the standard OpsWorks
security groups apply to created instances.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vpc<wbr>Id</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The id of the VPC that this stack belongs to.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## Import an Existing Stack Resource

TODO

## Support Types

#### StackCustomCookbooksSource

<table class="ml-6">
    <thead>
        <tr>
            <th>Argument</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="align-top">password</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">revision</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">ssh<wbr>Key</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">type</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">url</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) 
{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">username</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) 
{{% /md %}}</td>
        </tr>
    </tbody>
</table>
