# Marketing Funnel by Olist
https://www.kaggle.com/olistbr/marketing-funnel-olist

This is a marketing funnel dataset from sellers that filled-in requests of contact to sell their products on Olist Store. The dataset has information of 8k Marketing Qualified Leads (MQLs) that requested contact between Jun. 1st 2017 and Jun 1st 2018. They were randomly sampled from the total of MQLs. This is real data, it has been anonymized.

**Context**
This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners. See more on our website: www.olist.com

A seller join Olist through a marketing and sales funnel that was made public at this dataset. Description of steps:

1. Sign-up at a landing page.
2. Get contacted by a Sales development Representative (SDR), confirm some information and schedule a consultancy.
3. Consultancy is made by a Sales Representative (SR). The SR may close the deal (lead sing up) or lose the deal (led leaves without sign in)
4. Lead becomes a seller and starts building his catalog on Olist.
5. His products are published on marketplaces and ready to sell!

**Attention**
A seller MQL might come from multiple sources (he might subscribe on two different landing pages, for instance).

**olist_closed_deals_dataset.csv**
After a qualified lead fills in a form at a landing page he is contacted by a Sales Development Representative. At this step some information is checked and more information about the lead is gathered.
* mql_id: Marketing Qualified Lead id
* seller_id: Seller id
* sdr_id: Sales Development Representative id
* sr_id: Sales Representative id
* won_date: Date the deal was closed
* business_segment: Lead business segment. Informed on contact.
* lead_type: Lead type. Informed on contact.
* lead_behaviour_profile: Lead behaviour profile. SDR identify it on contact. https://www.discprofile.com/what-is-disc/overview/.
* *Shark - Dominance
* * Eagle - Influence
* * Cat - Steadiness
* *Wolf - Conscientiousness
* has_company: Does the lead have a company (formal documentation)?
* had_gtin: Does the lead have Global Trade Item Number (barcode) for his product?
* declared_product_catalog_size: Size of the product catalog
* declared_monthly_revenue: Monthly revenue of the seller
* average_stock: Average stock of the seller

**olist_marketing_qualified_lead_dataset.csv**
After a lead fills in a form at a landing page, a filter is made to select the ones that are qualified to sell their products at Olist. They are the Marketing Qualified Leads (MQLs).
* mql_id: Marketing Qualified Lead id
* first_contact_date: Date of the first contact solicitation.
* landing_page_id: Landing page id where the lead was acquired
* origin: Type of media where the lead was acquired
