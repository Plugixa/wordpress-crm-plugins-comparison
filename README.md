# WordPress CRM Plugins Compared

A sourced comparison of the maintained WordPress CRM plugins: FluentCRM, HubSpot, Jetpack CRM, WP ERP, Groundhogg, WP-CRM System and Plugixa CRM.

**Read it here: <https://plugixa.github.io/wordpress-crm-plugins-comparison/>** (English, Français, Español, Deutsch, Italiano)

Every value links to the vendor page it came from. Where a value could not be confirmed, the table says "Not checked".

> Maintained by [Plugixa](https://www.plugixa.com/), the makers of [Plugixa CRM](https://www.plugixa.com/plugins/plugixa-crm), one of the plugins compared. See the [methodology](https://plugixa.github.io/wordpress-crm-plugins-comparison/methodology/) for how that conflict of interest is handled.

<!-- generated:start -->
| Plugin | Best for | Active installs | Rating (count) | Paid from |
|---|---|---|---|---|
| [Plugixa CRM](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/plugixa-crm/) | Best free sales and service CRM | new | – | €39/yr |
| [HubSpot](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/hubspot/) | Best free hosted CRM | 200,000+ | 4.34 (207) | $84/yr |
| [FluentCRM](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/fluentcrm/) | Best for email marketing automation | 80,000+ | 4.77 (250) | $90/yr |
| [Jetpack CRM](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/jetpack-crm/) | Best for quotes and invoicing | 30,000+ | 4.32 (152) | $132/yr |
| [WP ERP](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/wp-erp/) | Best for HR and accounting together | 5,000+ | 4.38 (149) | $137/yr |
| [Groundhogg](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/groundhogg/) | Best for sales funnels and automation | 2,000+ | 4.87 (149) | $240/yr |
| [WP-CRM System](https://plugixa.github.io/wordpress-crm-plugins-comparison/plugins/wp-crm-system/) | Best for client and project tracking | 700+ | 3.93 (15) | $99/yr |
<!-- generated:end -->

Install counts and ratings come from the wordpress.org plugin API and are refreshed weekly.

## Pages

- [Full feature table](https://plugixa.github.io/wordpress-crm-plugins-comparison/#table)
- [Best WordPress CRM plugins](https://plugixa.github.io/wordpress-crm-plugins-comparison/best/best-wordpress-crm-plugins/)
- [Best free CRM plugins](https://plugixa.github.io/wordpress-crm-plugins-comparison/best/best-free-crm-plugins/)
- [CRM plugins with a sales pipeline](https://plugixa.github.io/wordpress-crm-plugins-comparison/best/crm-plugins-with-sales-pipeline/)
- [CRM plugins with email marketing](https://plugixa.github.io/wordpress-crm-plugins-comparison/best/crm-plugins-with-email-marketing/)
- [CRM plugins for WooCommerce](https://plugixa.github.io/wordpress-crm-plugins-comparison/best/crm-plugins-for-woocommerce/)
- [FluentCRM vs Groundhogg](https://plugixa.github.io/wordpress-crm-plugins-comparison/compare/fluentcrm-vs-groundhogg/)
- [HubSpot alternatives](https://plugixa.github.io/wordpress-crm-plugins-comparison/alternatives/hubspot/)

## Corrections

Found a wrong or outdated value? [Open an issue](https://github.com/Plugixa/wordpress-crm-plugins-comparison/issues/new) with a link to the vendor page that shows the correct one. Vendors are welcome to correct their own entries.

## How it works

| Path | Contents |
|---|---|
| `src/data/features.yaml` | The feature list |
| `src/data/products/*.yaml` | Facts per plugin; each checked value names its source |
| `src/data/wporg/*.json` | wordpress.org numbers, written by `npm run wporg` |
| `src/data/pages.yaml` | Which versus, alternatives and best-of pages exist |
| `src/i18n/{en,fr,es,de,it}/` | All text, one folder per language |

The build fails if a checked value has no source, or if a "partial" value has no note.

Plugixa CRM is not on wordpress.org yet, so it has no `wporg_slug` and shows as new. Add `wporg_slug: plugixa-crm` to `src/data/products/plugixa-crm.yaml` once it is listed.

```sh
npm install
npm run dev      # local preview
npm run wporg    # refresh wordpress.org numbers
npm run readme   # regenerate the table above
npm run build    # output in dist/
```

To publish under another address, change `SITE` and `BASE` in `astro.config.mjs`.

## Licence

Code: MIT. Data and text: CC BY 4.0. Plugin names are trademarks of their owners.
