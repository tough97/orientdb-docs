Find the top 3 Countries from where Customers are from:

In the _Browse Tab_ of [Studio](../../../studio/README.md), using the query below, this is the obtained list of records:

<pre><code class="lang-sql">SELECT 
  Name as CountryName,
  in('IsFromCountry').size() as NumberOfCustomers 
FROM Countries
ORDER BY NumberOfCustomers DESC 
LIMIT 3
</code></pre>

![](../../../images/demo-dbs/social-travel-agency/query_19_browse.png)