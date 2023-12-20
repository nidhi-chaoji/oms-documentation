# Introduction
{% hint style="info" %}
1. For information on previous releases, please consult the [previous document](https://docs.google.com/document/d/1lfvjpqBiE__1fsCjq7VvQSSXjdRLVZg86zJIXDDK-zc/edit). 
   
2. To find details about SOLR versions, refer to the [SOLR version document](https://docs.google.com/spreadsheets/d/1H-iEVG-hS9FTsYOf5YiUH-5KOJUcu0_TiPG8aVYjaHU/edit#gid=0).
{% endhint %}

This document provides details about all OMS releases created after December 1, 2023.

# Latest release

**Release Information**

| Information         | Value                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------------|
| Release Version     | v5.1.0                                                                                                  |
| Release Type        | Hotfix                                                                                                  |
| Image Tag           | v5.1.5                                                                                                  |
| Image URL           | (289432782788.dkr.ecr.us-east-1.amazonaws.com/omscoreimage:omscoreimage-v5.1.5)                         |
| Diff                | NA                                                                                                      |
| Changelog           | NA                                       |


{% tabs %}

{% tab title="Upgrade Data" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeData.xml?ref_type=tags">Link to Upgrade Data</a>{% endtab %}

{% tab title="Upgrade SQL" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeSQL.sql?ref_type=tags">Link to Upgrade SQL</a> {% endtab %}

{% tab title="Upgrade Steps" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeSteps.md?ref_type=tags">Link to Upgrade Steps</a> {% endtab %}

{% endtabs %}


# Old release

**Release Information**

| Information         | Value                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------------|
| Release Version     | v5.1.0                                                                                                  |
| Release Type        | Minor                                                                                                |
| Image Tag           | v5.1.0                                                                                                  |
| Image URL           | `289432782788.dkr.ecr.us-east-1.amazonaws.com/omscoreimage:omscoreimage-v5.1.0`                           |
| Diff                | [Link to Difference](https://git.hotwax.co/commerce/oms/-/compare/v5.0.0...v5.1.0?from_project_id=161&straight=false)         |
| Changelog           | [Link to Changelog](https://git.hotwax.co/commerce/oms/-/blob/main/CHANGELOG.md)                                       |


{% tabs %}

{% tab title="Upgrade Data" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeSteps.md?ref_type=tags">Link to Upgrade Steps</a>
{% endtab %}

{% tab title="Upgrade SQL" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeSQL.sql?ref_type=tags">Link to Upgrade SQL</a> {% endtab %}

{% tab title="Upgrade Steps" %} <a href="https://git.hotwax.co/commerce/oms/-/blob/v5.1.0/applications/hwmapps/upgrade/current/UpgradeSteps.md?ref_type=tags">Link to Upgrade Steps</a> {% endtab %}

{% endtabs %}


# Optional Plugins

| Plugin            | Version | Repository                                                    |
|-------------------|---------|---------------------------------------------------------------|
| **netsuite**      | v4.16.0 | [netsuite](https://git.hotwax.co/plugins/netsuite.git)       |
| **klaviyo**       | v4.12.0 | [klaviyo](https://git.hotwax.co/plugins/klaviyo.git)         |
| **shipstation**   | v4.12.0 | [shipstation](https://git.hotwax.co/plugins/shipping-integrations/shipstation.git) |
| **shipt**         | v4.12.0 | [shipt](https://git.hotwax.co/plugins/shipping-integrations/shipt.git) |
| **c807**          | v4.19.0 | [c807](https://git.hotwax.co/plugins/shipping-integrations/c807.git) |
| **guatex**        | v4.19.0 | [guatex](https://git.hotwax.co/plugins/shipping-integrations/guatex.git) |
| **terminal-express** | v4.19.0 | [terminal-express](https://git.hotwax.co/plugins/shipping-integrations/terminal-express.git) |
| **cargotrans**    | v4.19.0 | [cargotrans](https://git.hotwax.co/plugins/shipping-integrations/cargotrans.git) |