# Google Document AI Client for Java

Java idiomatic client for [Document AI][product-docs].

[![Maven][maven-version-image]][maven-version-link]
![Stability][stability-image]

- [Product Documentation][product-docs]
- [Client Library Documentation][javadocs]

## Quickstart

If you are using Maven with [BOM][libraries-bom], add this to your pom.xml file
```xml
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>com.google.cloud</groupId>
      <artifactId>libraries-bom</artifactId>
      <version>20.8.0</version>
      <type>pom</type>
      <scope>import</scope>
    </dependency>
  </dependencies>
</dependencyManagement>

<dependencies>
  <dependency>
    <groupId>com.google.cloud</groupId>
    <artifactId>google-cloud-document-ai</artifactId>
    <version>1.2.1</version>
  </dependency>

```

If you are using Maven without BOM, add this to your dependencies:

```xml
<dependency>
  <groupId>com.google.cloud</groupId>
  <artifactId>google-cloud-document-ai</artifactId>
  <version>1.2.1</version>
</dependency>

```

If you are using Gradle 5.x or later, add this to your dependencies
```Groovy
implementation platform('com.google.cloud:libraries-bom:20.8.0')

compile 'com.google.cloud:google-cloud-document-ai'
```
If you are using Gradle without BOM, add this to your dependencies
```Groovy
compile 'com.google.cloud:google-cloud-document-ai:1.2.1'
```

If you are using SBT, add this to your dependencies
```Scala
libraryDependencies += "com.google.cloud" % "google-cloud-document-ai" % "1.2.1"
```

## Authentication

See the [Authentication][authentication] section in the base directory's README.

## Getting Started

### Prerequisites

You will need a [Google Cloud Platform Console][developer-console] project with the Document AI [API enabled][enable-api].
You will need to [enable billing][enable-billing] to use Google Document AI.
[Follow these instructions][create-project] to get your project set up. You will also need to set up the local development environment by
[installing the Google Cloud SDK][cloud-sdk] and running the following commands in command line:
`gcloud auth login` and `gcloud config set project [YOUR PROJECT ID]`.

### Installation and setup

You'll need to obtain the `google-cloud-document-ai` library.  See the [Quickstart](#quickstart) section
to add `google-cloud-document-ai` as a dependency in your code.

## About Document AI


[Document AI][product-docs] allows developers to unlock insights from your documents with machine learning.

See the [Document AI client library docs][javadocs] to learn how to
use this Document AI Client Library.





## Samples

Samples are in the [`samples/`](https://github.com/googleapis/java-document-ai/tree/master/samples) directory. The samples' `README.md`
has instructions for running the samples.

| Sample                      | Source Code                       | Try it |
| --------------------------- | --------------------------------- | ------ |
| Batch Process Document | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1/BatchProcessDocument.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1/BatchProcessDocument.java) |
| Process Document | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1/ProcessDocument.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1/ProcessDocument.java) |
| Quick Start | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1/QuickStart.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1/QuickStart.java) |
| Batch Parse Form Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/BatchParseFormBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/BatchParseFormBeta.java) |
| Batch Parse Table Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/BatchParseTableBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/BatchParseTableBeta.java) |
| Parse Form Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/ParseFormBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/ParseFormBeta.java) |
| Parse Table Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/ParseTableBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/ParseTableBeta.java) |
| Parse With Model Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/ParseWithModelBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/ParseWithModelBeta.java) |
| Quick Start | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/QuickStart.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/QuickStart.java) |
| Set End Point Beta | [source code](https://github.com/googleapis/java-document-ai/blob/master/samples/snippets/src/main/java/documentai/v1beta2/SetEndPointBeta.java) | [![Open in Cloud Shell][shell_img]](https://console.cloud.google.com/cloudshell/open?git_repo=https://github.com/googleapis/java-document-ai&page=editor&open_in_editor=samples/snippets/src/main/java/documentai/v1beta2/SetEndPointBeta.java) |



## Troubleshooting

To get help, follow the instructions in the [shared Troubleshooting document][troubleshooting].

## Transport

Document AI uses gRPC for the transport layer.

## Supported Java Versions

Java 7 or above is required for using this client.

Google's Java client libraries,
[Google Cloud Client Libraries][cloudlibs]
and
[Google Cloud API Libraries][apilibs],
follow the
[Oracle Java SE support roadmap][oracle]
(see the Oracle Java SE Product Releases section).

### For new development

In general, new feature development occurs with support for the lowest Java
LTS version covered by  Oracle's Premier Support (which typically lasts 5 years
from initial General Availability). If the minimum required JVM for a given
library is changed, it is accompanied by a [semver][semver] major release.

Java 11 and (in September 2021) Java 17 are the best choices for new
development.

### Keeping production systems current

Google tests its client libraries with all current LTS versions covered by
Oracle's Extended Support (which typically lasts 8 years from initial
General Availability).

#### Legacy support

Google's client libraries support legacy versions of Java runtimes with long
term stable libraries that don't receive feature updates on a best efforts basis
as it may not be possible to backport all patches.

Google provides updates on a best efforts basis to apps that continue to use
Java 7, though apps might need to upgrade to current versions of the library
that supports their JVM.

#### Where to find specific information

The latest versions and the supported Java versions are identified on
the individual GitHub repository `github.com/GoogleAPIs/java-SERVICENAME`
and on [google-cloud-java][g-c-j].

## Versioning


This library follows [Semantic Versioning](http://semver.org/).


## Contributing


Contributions to this library are always welcome and highly encouraged.

See [CONTRIBUTING][contributing] for more information how to get started.

Please note that this project is released with a Contributor Code of Conduct. By participating in
this project you agree to abide by its terms. See [Code of Conduct][code-of-conduct] for more
information.

## License

Apache 2.0 - See [LICENSE][license] for more information.

## CI Status

Java Version | Status
------------ | ------
Java 7 | [![Kokoro CI][kokoro-badge-image-1]][kokoro-badge-link-1]
Java 8 | [![Kokoro CI][kokoro-badge-image-2]][kokoro-badge-link-2]
Java 8 OSX | [![Kokoro CI][kokoro-badge-image-3]][kokoro-badge-link-3]
Java 8 Windows | [![Kokoro CI][kokoro-badge-image-4]][kokoro-badge-link-4]
Java 11 | [![Kokoro CI][kokoro-badge-image-5]][kokoro-badge-link-5]

Java is a registered trademark of Oracle and/or its affiliates.

[product-docs]: https://cloud.google.com/compute/docs/documentai/
[javadocs]: https://googleapis.dev/java/google-cloud-document-ai/latest/index.html
[kokoro-badge-image-1]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java7.svg
[kokoro-badge-link-1]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java7.html
[kokoro-badge-image-2]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8.svg
[kokoro-badge-link-2]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8.html
[kokoro-badge-image-3]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8-osx.svg
[kokoro-badge-link-3]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8-osx.html
[kokoro-badge-image-4]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8-win.svg
[kokoro-badge-link-4]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java8-win.html
[kokoro-badge-image-5]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java11.svg
[kokoro-badge-link-5]: http://storage.googleapis.com/cloud-devrel-public/java/badges/java-document-ai/java11.html
[stability-image]: https://img.shields.io/badge/stability-ga-green
[maven-version-image]: https://img.shields.io/maven-central/v/com.google.cloud/google-cloud-document-ai.svg
[maven-version-link]: https://search.maven.org/search?q=g:com.google.cloud%20AND%20a:google-cloud-document-ai&core=gav
[authentication]: https://github.com/googleapis/google-cloud-java#authentication
[developer-console]: https://console.developers.google.com/
[create-project]: https://cloud.google.com/resource-manager/docs/creating-managing-projects
[cloud-sdk]: https://cloud.google.com/sdk/
[troubleshooting]: https://github.com/googleapis/google-cloud-common/blob/master/troubleshooting/readme.md#troubleshooting
[contributing]: https://github.com/googleapis/java-document-ai/blob/master/CONTRIBUTING.md
[code-of-conduct]: https://github.com/googleapis/java-document-ai/blob/master/CODE_OF_CONDUCT.md#contributor-code-of-conduct
[license]: https://github.com/googleapis/java-document-ai/blob/master/LICENSE
[enable-billing]: https://cloud.google.com/apis/docs/getting-started#enabling_billing
[enable-api]: https://console.cloud.google.com/flows/enableapi?apiid=documentai.googleapis.com
[libraries-bom]: https://github.com/GoogleCloudPlatform/cloud-opensource-java/wiki/The-Google-Cloud-Platform-Libraries-BOM
[shell_img]: https://gstatic.com/cloudssh/images/open-btn.png

[semver]: https://semver.org/
[cloudlibs]: https://cloud.google.com/apis/docs/client-libraries-explained
[apilibs]: https://cloud.google.com/apis/docs/client-libraries-explained#google_api_client_libraries
[oracle]: https://www.oracle.com/java/technologies/java-se-support-roadmap.html
[g-c-j]: http://github.com/googleapis/google-cloud-java
