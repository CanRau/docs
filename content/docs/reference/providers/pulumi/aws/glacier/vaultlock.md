---
title: "VaultLock"
---

<!-- WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

<style>
  table td p { margin-top: 0; margin-bottom: 0; }
</style>

Manages a Glacier Vault Lock. You can refer to the [Glacier Developer Guide](https://docs.aws.amazon.com/amazonglacier/latest/dev/vault-lock.html) for a full explanation of the Glacier Vault Lock functionality.

> **NOTE:** This resource allows you to test Glacier Vault Lock policies by setting the `complete_lock` argument to `false`. When testing policies in this manner, the Glacier Vault Lock automatically expires after 24 hours and this provider will show this resource as needing recreation after that time. To permanently apply the policy, set the `complete_lock` argument to `true`. When changing `complete_lock` to `true`, it is expected the resource will show as recreating.

!> **WARNING:** Once a Glacier Vault Lock is completed, it is immutable. The deletion of the Glacier Vault Lock is not be possible and attempting to remove it from this provider will return an error. Set the `ignore_deletion_error` argument to `true` and apply this configuration before attempting to delete this resource via this provider or remove this resource from this provider's management.

> This content is derived from https://github.com/terraform-providers/terraform-provider-aws/blob/master/website/docs/r/glacier_vault_lock.html.markdown.


## Create a VaultLock Resource

{{< langchoose csharp >}}

<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new</span> <span class="nx"><a href=/docs/reference/pkg/nodejs/pulumi/aws/s3/#VaultLock>VaultLock</a></span><span class="p">(</span><span class="nx">name</span>: <span class="kt"><a href=https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String>string</a></span><span class="p">,</span> <span class="nx">args</span>: <span class="kt"><a href=/docs/reference/pkg/nodejs/pulumi/aws/s3/#VaultLockArgs>VaultLockArgs</a></span><span class="p">,</span> <span class="nx">opts?</span>: <span class="kt"><a href=/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions>pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>

```python
def __init__(__self__, resource_name, opts=None, complete_lock=None, ignore_deletion_error=None, policy=None, vault_name=None, __props__=None)
```

```go
func NewVaultLock(ctx *pulumi.Context, name string, args *VaultLockArgs, opts ...pulumi.ResourceOption) (*VaultLock, error)

```

```csharp
public VaultLock(string name, VaultLockArgs args, CustomResourceOptions? options = null)

```

Creates a VaultLock resource with the given unique name, arguments, and options.

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
            <td class="align-top">complete<wbr>Lock</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Required) Boolean whether to permanently apply this Glacier Lock Policy. Once completed, this cannot be undone. If set to `false`, the Glacier Lock Policy remains in a testing mode for 24 hours. After that time, the Glacier Lock Policy is automatically removed by Glacier and the this provider resource will show as needing recreation. Changing this from `false` to `true` will show as resource recreation, which is expected. Changing this from `true` to `false` is not possible unless the Glacier Vault is recreated at the same time.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">ignore<wbr>Deletion<wbr>Error</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Allow this provider to ignore the error returned when attempting to delete the Glacier Lock Policy. This can be used to delete or recreate the Glacier Vault via this provider, for example, if the Glacier Vault Lock policy permits that action. This should only be used in conjunction with `complete_lock` being set to `true`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">policy</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) JSON string containing the IAM policy to apply as the Glacier Vault Lock policy.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vault<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Required) The name of the Glacier Vault.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## VaultLock Output Properties

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
            <td class="align-top">complete<wbr>Lock</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
Boolean whether to permanently apply this Glacier Lock Policy. Once completed, this cannot be undone. If set to `false`, the Glacier Lock Policy remains in a testing mode for 24 hours. After that time, the Glacier Lock Policy is automatically removed by Glacier and the this provider resource will show as needing recreation. Changing this from `false` to `true` will show as resource recreation, which is expected. Changing this from `true` to `false` is not possible unless the Glacier Vault is recreated at the same time.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">ignore<wbr>Deletion<wbr>Error</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
Allow this provider to ignore the error returned when attempting to delete the Glacier Lock Policy. This can be used to delete or recreate the Glacier Vault via this provider, for example, if the Glacier Vault Lock policy permits that action. This should only be used in conjunction with `complete_lock` being set to `true`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">policy</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
JSON string containing the IAM policy to apply as the Glacier Vault Lock policy.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vault<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
The name of the Glacier Vault.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## Look up an Existing VaultLock Resource

{{< langchoose csharp >}}

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: VaultLockState, opts?: pulumi.CustomResourceOptions): VaultLock;
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

Get an existing VaultLock resource's state with the given name, ID, and optional extra
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
            <td class="align-top">complete<wbr>Lock</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Boolean whether to permanently apply this Glacier Lock Policy. Once completed, this cannot be undone. If set to `false`, the Glacier Lock Policy remains in a testing mode for 24 hours. After that time, the Glacier Lock Policy is automatically removed by Glacier and the this provider resource will show as needing recreation. Changing this from `false` to `true` will show as resource recreation, which is expected. Changing this from `true` to `false` is not possible unless the Glacier Vault is recreated at the same time.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">ignore<wbr>Deletion<wbr>Error</td>
            <td class="align-top"><code>boolean</code></td>
            <td class="align-top">{{% md %}}
(Optional) Allow this provider to ignore the error returned when attempting to delete the Glacier Lock Policy. This can be used to delete or recreate the Glacier Vault via this provider, for example, if the Glacier Vault Lock policy permits that action. This should only be used in conjunction with `complete_lock` being set to `true`.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">policy</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) JSON string containing the IAM policy to apply as the Glacier Vault Lock policy.

{{% /md %}}</td>
        </tr>
        <tr>
            <td class="align-top">vault<wbr>Name</td>
            <td class="align-top"><code>string</code></td>
            <td class="align-top">{{% md %}}
(Optional) The name of the Glacier Vault.

{{% /md %}}</td>
        </tr>
    </tbody>
</table>

## Import an Existing VaultLock Resource

TODO

## Support Types
