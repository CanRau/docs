---
layout: "home"
noindex: true
---

<div class="text-center">
    <img class="inline max-w-xs" src="/images/logo/logo.svg" alt="Pulumi logo">
    <h2>
        Cloud Native Infrastructure as Code
    </h2>
    <h3>
        Provision infrastructure on any cloud using your favorite language.
    </h3>
    <p class="md:flex justify-center">
        <a class="block btn mx-1 my-1" href="{{< relref "/docs/quickstart/install.md" >}}">INSTALL</a>
        <a class="block btn mx-1 my-1" href="{{< relref "/docs/quickstart" >}}">GET STARTED</a>
        <a class="block btn mx-1 my-1" href="{{< relref "/docs/reference" >}}">LEARN</a>
    </p>
</div>

<div class="my-4 bg-gray-lightest border-t border-b border-gray-light md:flex py-8 px-32">
    <a href="{{< relref "/docs/quickstart/aws" >}}"><img src="/images/docs/quickstart/aws-purple.png"></a>
    <a href="{{< relref "/docs/quickstart/azure" >}}"><img src="/images/docs/quickstart/azure-purple.png"></a>
    <a href="{{< relref "/docs/quickstart/gcp" >}}"><img src="/images/docs/quickstart/gcp-purple.png"></a>
    <a href="{{< relref "/docs/quickstart/kubernetes" >}}"><img src="/images/docs/quickstart/k8s-purple.png"></a>
</div>

<div class="my-4 md:flex py-8 px-32">
    <div>
        <h3>Why Pulumi?</h3>
        <p>
            By using general purpose languages for infrastructure as code,
            you get all the benefits of real languages -- IDEs, abstractions and
            reuse thanks to functions, classes, and packages, debugging, testability,
            and more. The result is far less copy and paste and greater productivity,
            and it works the same way no matter which cloud you're targeting.
        </p>
    </div>
    <div>
        <h3>Alternatives</h3>
        <p>
            Other approaches use YAML, JSON, or bespoke DSLs that you need to
            master -- and convince your team to use. These "languages" fall short of
            general purpose languages, lacking abstractions and reuse, and reinvent
            familiar concepts like package managers. Worse, these solutions are usually
            unique to every given cloud that you need to target.
        </p>
    </div>
    <div>
        <h3>Community</h3>
        <p>
            Pulumi's SDK is fully open source and extensible, enabling you to
            participate in a rich ecosystem of libraries that ease common tasks,
            ranging from containers to serverless to infrastructure, and everything
            in between. Languages and clouds are supported using an extensible
            plugin model, enabling public, private, and even hybrid cloud support.
        </p>
    </div>
</div>

<div class="my-4 bg-gray-lightest border-t border-b border-gray-light md:flex py-8 px-32">
    <div class="text-center">
        <a href="{{< relref "/docs/quickstart/aws/tutorial-service" >}}">
            <img class="inline h-32" src="/images/docs/icon-feature-containers.svg">
            <h3>Containers</h3>
        </a>
        <p>
            Deploy a Docker container to production in 5 minutes using your favorite orchestrator.
        </p>
        <a class="btn" href="{{< relref "/docs/quickstart/aws/tutorial-service.md" >}}">
            START NOW
        </a>
    </div>
    <div class="text-center">
        <a href="{{< relref "/docs/quickstart/aws/tutorial-rest-api" >}}">
            <img class="inline h-32" src="/images/docs/icon-feature-serverless.svg">
            <h3>Serverless</h3>
        </a>
        <p>
            Stand up a serverless API or event handler in 5 minutes using a real lambda in code.
        </p>
        <a class="btn" href="{{< relref "/docs/quickstart/aws/tutorial-rest-api.md" >}}">
            START NOW
        </a>
    </div>
    <div class="text-center">
        <a href="{{< relref "/docs/quickstart/aws/tutorial-ec2-webserver" >}}">
            <img class="inline h-32" src="/images/docs/icon-feature-data.svg">
            <h3>Infrastructure</h3>
        </a>
        <p>
            Manage cloud infrastructure or hosted services using infrastructure as code.
        </p>
        <a class="btn" href="{{< relref "/docs/quickstart/aws/tutorial-ec2-webserver" >}}">
            START NOW
        </a>
    </div>
    <div class="text-center">
        <a href="{{< relref "/docs/quickstart/kubernetes" >}}">
            <img class="inline h-32" src="/images/docs/icon-feature-kubernetes.svg">
            <h3>Kubernetes</h3>
        </a>
        <p>
            Deploy and orchestrate cloud native Kubernetes services in real code, no YAML needed.
        </p>
        <a class="btn" href="{{< relref "/docs/quickstart/kubernetes" >}}">
            START NOW
        </a>
    </div>
</div>

For questions or feedback, reach us in our [community Slack channel](https://slack.pulumi.io),
on [GitHub](https://github.com/pulumi), or by emailing [support@pulumi.com](mailto:support@pulumi.com).