---
title: Java JDKs and long-term support for Azure development
description: Downloads and statement of Azure support for developing and running Java applications.
author: bmitchell287
manager: douge
ms.devlang: java
ms.topic: article
ms.date: 04/09/2019
ms.author: brendm
ms.topic: conceptual
---

# Get Java JDK downloads and support when developing for Azure

Java developers on Azure and Azure Stack can build and run production Java applications using [Azul Zulu Enterprise for Azure](https://www.azul.com/downloads/azure-only/zulu/) without incurring additional support costs. You can use any Java runtime you want on Azure, but when you use Zulu you get free maintenance updates and can create support issues with Microsoft with a  [qualified Azure support plan](https://azure.microsoft.com/support/plans/).

Download JDK distributions now.

**Long term support (LTS)**

- [Java 11](https://www.azul.com/downloads/azure-only/zulu/#java11)
- [Java 8](https://www.azul.com/downloads/azure-only/zulu/#java8)
- [Java 7](https://www.azul.com/downloads/azure-only/zulu/#java7)

**Technical preview**

- [Java 12](https://www.azul.com/downloads/azure-only/zulu/#java12)

Developers can also use their own Java run-times, including Oracle JDK and Red Hat JDK, to run their apps on Azure and connect to Azure services and features. The production edition of Oracle Java SE continues to be available to Java developers running  workloads in Azure Windows or Linux virtual machines.

## What is the Zulu OpenJDK for Azure?
Azul Zulu Enterprise Builds of OpenJDK are a no cost, multi-platform, production ready distribution of the OpenJDK for Azure and Azure Stack backed by Microsoft and Azul Systems. These distributions are:

- 100% open source builds of OpenJDK packaged as Java Development Kits (JDKs), Java Runtime Environments (JREs), and Headless JREs. These binaries are fully compatible and compliant commercial builds of Java Standard Edition (SE) that can be used with Java applications or components on Azure and Azure Stack.
- Provided with long-term support including bug fixes, performance enhancements, and security patches.
- Available for developing and running Java applications on Windows, Linux, and MacOS.
- Available as container images on Docker Hub and as virtual machines (Windows and Linux) on Azure Marketplace.
- Used by Microsoft Azure to power many Azure services, such as:
  - App Service Windows
  - App Service Linux
  - Functions
  - Service Fabric
  - HDInsight
  - Search
  - Azure DevOps
  - Cloud Shell  

## Supported Java versions and update schedule

Azul Systems provides fully-supported [Zulu Enterprise builds of OpenJDK for Microsoft Azure](https://www.azul.com/downloads/azure-only/zulu/) for all long-term support (LTS) versions of Java, starting with Java SE 7, 8, and 11. More information can be found in the [Azul press release](https://www.azul.com/press_release/free-java-production-support-for-microsoft-azure-azure-stack).


|Java SE LTS  |Support until  |
|---------|----------|
|Java 7   |July 2023 |
|Java 8   |March 2025|
|Java 11  |Sept. 2026|

These JDK releases have quarterly security updates, bug fixes, and critical out-of-band updates and patches as needed.  This support includes back ports of security updates and bug fixes to Java 7 and 8 reported in newer versions of Java such as Java 11, which ensures the continued stability and security of older versions of Java.  Azure customers can get these security updates and platform bug fixes without incurring any unplanned Java SE subscription fees. The dates of support for each version of Java SE are highlighted in the image below.

![JDK support timeline for Azure](../media/azure-jdk-support.png)

Azul Systems maintains a [Java SE roadmap](https://www.azul.com/products/azul_support_roadmap/) for these releases.

## Benefits for developers

The Azul Zulu JDK releases are:

1. Backed and supported by both Microsoft and Azul Systems
    - Zulu binaries are production-ready and backed by Microsoft and Azul Systems
    - Zulu comes with zero-cost long-term support (LTS) for Java 7, 8, and 11. (LTS will be provided for Java 17, as well). You can upgrade Java versions only when you need to.
    - Java 7 supported until July 2023. Java 8 and 11 are supported beyond 2024.
    - Microsoft is committed to running Zulu internally on machines that power many Azure services.
2. Production-ready
    - 100% open-source for its builds of OpenJDK.
    - Drop-in replacements for many Java SE distributions.
      - JDK, JRE, and JRE-headless
      - Java 7, 8, and 11
    - Verified compliant with the Java SE  specifications using the OpenJDK Community Technology Compatibility Kit (TCK).
    - Developers will continue to receive production updates for Java SE, including bug fixes, performance enhancements, and security patches for Java SE 7, 8, and 11.
3. Supported for multi-platform. Zulu supports binaries for multiple platforms and versions, including:
   - Windows Client
     - 10
     - 10 IoT Core
     - 8.1
     - 8, 7
   - Windows Server
     - 2016R2
     - 2016
     - 2012R2
     - 2012
     - 2008R2
   - Linux, including
     - RHEL
     - CentOS
     - Ubuntu
     - SLES
     - Debian
     - Oracle Linux
   - Mac OS X
     - delivered in multiple package types:
     - MSI, ZIP, TAR, DEB, RPM, and DMG
   - Certified Docker container images for Zulu JDK, JRE, and JRE-headless on multiple base OS images are available at Docker Hub:
     - [JDK](https://hub.docker.com/_/microsoft-java-jdk)
     - [JRE](https://hub.docker.com/_/microsoft-java-jre)
     - [JRE-headless](https://hub.docker.com/_/microsoft-java-jre-headless)
4. No cost
   - Microsoft provides everything you need to build and scale Java apps on Azure at no cost to you. Through Zulu you'll receive free security updates and platform bug fixes for Java apps without any fees.
   - Java Flight Recorder and Mission Control are available in Zulu Java 8, 11, and beyond.
5. Tech Preview of Non-LTS versions
   - Tech previews provide you with opportunities to progressively test new features as they are delivered in short-term versions that will eventually graduate to Java 17 LTS.
6. Changes to OpenJDK are up-streamed
   - Azul Systems committers push Zulu changes to OpenJDK which makes the upstream repo comprehensive and inclusive.

As always, Java developers can bring their own Java run-times, including Oracle JDK and Red Hat JDK, to Azure and use  the secure infrastructure and feature-rich services. The production edition of Oracle Java SE is also available to Java developers for running Java workloads in Windows or Linux virtual machines on Azure.

## Use for local development 

Developers can [download](https://www.azul.com/downloads/azure-only/zulu/) Java JDKs for Azure and Azure Stack for use in local devlopment environments. Downloads are available for Windows, Linux, and macOS. Developers working on Linux can also get packages through the [yum](https://www.azul.com/downloads/azure-only/zulu/#yum-repo) and [apt](https://www.azul.com/downloads/azure-only/zulu/#apt-repo) package managers.

When developing for Azure or Azure Stack, support for local development with a JDK is available with a [qualified Azure support plan](https://azure.microsoft.com/support/plans/).

## Use in Docker containers

You can build unlimited Docker images using Zulu Enterprise builds of OpenJDK on any distros of your choice. Zulu Docker images based off the Azul Zulu Enterprise for Azure JDKs are available on [Microsoft's public Docker repository](https://hub.docker.com/r/microsoft/java-jdk/). The Dockerfiles used to build these images are available on [Microsoft's Java GitHub repo](https://github.com/Microsoft/java/tree/master/docker).

To containerize your apps using these images,  set a `FROM` statement in your Dockerfile and then configure the container with your application's dependencies. For example, to run a JAR file packaged Java SE application that binds to port 8080:

```Dockerfile
FROM  microsoft/java-jdk:<tag>
EXPOSE 8080
ADD target/hello.jar hello.jar
ENTRYPOINT ["java", "-jar","/hello.jar"]
```

For additional guidance see [Docker images for Azure](java-jdk-docker-images.md).

## Azure service runtime support

Azure platform services such as [App Service](/azure/app-service/containers/), [Functions](/azure/azure-functions/functions-create-first-java-maven), [Service Fabric](/azure/service-fabric/) and [HDInsight](/azure/hdinsight/)  use Zulu Enterprise builds of OpenJDK with built-in auto-patching of minor releases of Java, including security patches and bug fixes.