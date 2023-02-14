## Overview

Glue42 Server is a server-side app that provides data to Glue42 (apps, Layouts, preferences) and allows monitoring and interacting with users running Glue42.

It also includes an Admin UI that helps managing the data stored in the Glue42 Server easier.

<glue42 name="diagram" image="../../../images/glue42-server/server-architecture.png">

## Features

#### App Store

The Glue42 Server provides an [app definition store](https://docs.glue42.com/glue42-concepts/application-management/overview/index.html#app_stores) that can be used by [**Glue42 Enterprise**](https://glue42.com/enterprise/) and [**Glue42 Core+**](https://glue42.com/core-plus/) projects to retrieve the list of apps for the current user.

#### Layout Store

The Glue42 Server is a [Layout store](https://docs.glue42.com/glue42-concepts/windows/layouts/overview/index.html#layout_stores) from where common or private user Layouts can be fetched for [**Glue42 Enterprise**](https://glue42.com/enterprise/) and [**Glue42 Core+**](https://glue42.com/core-plus/) projects.

#### App Preferences Store

The Glue42 Server is an [app preferences](https://docs.glue42.com/glue42-concepts/app-preferences/overview/index.html) store where any app running in [**Glue42 Enterprise**](https://glue42.com/enterprise/) can store custom data per user and retrieve it later.

#### Configurations Store

The Glue42 Server can host and supply all [configuration files](https://docs.glue42.com/developers/configuration/overview/index.html) for [**Glue42 Enterprise**](https://glue42.com/enterprise/). Different versions of the configuration files can be provided for different versions of [**Glue42 Enterprise**](https://glue42.com/enterprise/).

#### Diagnostics

The Glue42 Server comes with an Admin UI which offers the following functionalities:

- Command Center - send commands to specific user sessions for getting logs, triggering page refresh, restarting the desktop client or even executing custom code;
- Feedback and Native Crashes - monitor, review and comment user Feedback and Native Crashes reports;
- User Monitoring - monitor users and their sessions (current and closed), inspect their hardware setup;