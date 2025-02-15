{% ifversion ghes = 2.22 %}

{% note %}

**Note**: If you joined the beta for {% data variables.product.prodname_actions %} or {% data variables.product.prodname_registry %} and enabled the features, your instance requires additional hardware resources. Minimum requirements for an instance with beta features enabled are **bold** in the following table. For more information, see "[Beta features in {% data variables.product.prodname_ghe_server %} 2.22](#beta-features-in-github-enterprise-server-222)."

{% endnote %}

{% endif %}

{% ifversion ghes > 2.22 %}

| User licenses | vCPUs | Memory | Attached storage | Root storage |
| :- | -: | -: | -: | -: |
| Trial, demo, or 10 light users | 4 | 32 GB | 150 GB | 200 GB |
| 10 to 3,000  | 8 | 48 GB | 300 GB | 200 GB |
| 3,000 to 5000 | 12 | 64 GB | 500 GB | 200 GB |
| 5,000 to 8000 | 16 | 96 GB | 750 GB | 200 GB |
| 8,000 to 10,000+ | 20 | 160 GB | 1000 GB | 200 GB |

{% else %}

| User licenses | vCPUs | Memory | Attached storage | Root storage |
| :- | -: | -: | -: | -: |
| Trial, demo, or 10 light users | 2{% ifversion ghes = 2.22 %}<br/>or [**4**](#beta-features-in-github-enterprise-server-222){% endif %} | 16 GB{% ifversion ghes = 2.22 %}<br/>or [**32 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 100 GB{% ifversion ghes = 2.22 %}<br/>or [**150 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 200 GB |
| 10 to 3,000  | 4{% ifversion ghes = 2.22 %}<br/>or [**8**](#beta-features-in-github-enterprise-server-222){% endif %} | 32 GB{% ifversion ghes = 2.22 %}<br/>or [**48 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 250 GB{% ifversion ghes = 2.22 %}<br/>or [**300 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 200 GB |
| 3,000 to 5000 | 8{% ifversion ghes = 2.22 %}<br/>or [**12**](#beta-features-in-github-enterprise-server-222){% endif %} | 64 GB | 500 GB | 200 GB |
| 5,000 to 8000 | 12{% ifversion ghes = 2.22 %}<br/>or [**16**](#beta-features-in-github-enterprise-server-222){% endif %} | 96 GB | 750 GB | 200 GB |
| 8,000 to 10,000+ | 16{% ifversion ghes = 2.22 %}<br/>or [**20**](#beta-features-in-github-enterprise-server-222){% endif %} | 128 GB{% ifversion ghes = 2.22 %}<br/>or [**160 GB**](#beta-features-in-github-enterprise-server-222){% endif %} | 1000 GB | 200 GB |

{% endif %}

{% data reusables.enterprise_installation.root-disk-partition %}

{% ifversion ghes > 2.22 %}

If you plan to enable {% data variables.product.prodname_actions %} for the users of your instance, review the requirements for hardware, external storage, and runners in "[Getting started with {% data variables.product.prodname_actions %} for {% data variables.product.prodname_ghe_server %}](/admin/github-actions/getting-started-with-github-actions-for-github-enterprise-server)."

{% endif %}

{% data reusables.enterprise_installation.about-adjusting-resources %}

{% ifversion ghes = 2.22 %}

### Beta features in {% data variables.product.prodname_ghe_server %} 2.22

{% data variables.product.prodname_ghe_server %} 2.22 offered features in beta, such as {% data variables.product.prodname_actions %}, {% data variables.product.prodname_registry %}, and {% data variables.product.prodname_code_scanning %}. For more information, see the [{% data variables.product.prodname_ghe_server %} 2.22 release notes](/enterprise-server@2.22/admin/release-notes#2.22.0).

If you enabled beta features for {% data variables.product.prodname_ghe_server %} 2.22, your instance requires additional hardware resources. For more information about minimum requirements, see "[Minimum requirements](#minimum-requirements)."

For more information about the hardware requirements for {% data variables.product.prodname_actions %}, see "[Getting started with {% data variables.product.prodname_actions %} for {% data variables.product.prodname_ghe_server %}](/admin/github-actions/getting-started-with-github-actions-for-github-enterprise-server#review-hardware-considerations)."

{% endif %}
