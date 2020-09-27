# prov_quotas
Gender Quotas in Argentine Provinces, 1992-2020
===============================================

Last update:
------------------
09-25-2020

The election of local authorities in Argentina is significantly decentralized: province-level elections are ruled by provincial constitutions and provincial laws, while national laws have limited influence over them. The adoption of gender quotas in early 1990s substantively increased the number of elected women at the Argentine Congress (Jones 1996; Lubertino 2003; Alles 2007). However, the gender quotas adopted for national elections, though may have inspired local emulations, do not affect provincial elections.

Provinces have implemented (and enforced) their own gender quotas, passing quite different versions of them: some adopted loose requirements, some enforced strict ones, some introduced them many years later (Caminotti 2014).

The <b>first wave</b> of adoption occurred during the 1990s. La Rioja and Santa Fe were the earliest adopters in 1992, and by 1995, more than half of the provinces had passed pieces of legislation requiring the inclusion of at least a third of female candidates in party lists. Since then, every province has adopted some form of gender quota.

The <b>second wave</b> of reforms, though there were a few early adoptions during the 2000s (Cordoba, Santiago del Estero, Rio Negro), started in the late 2010s, and it is still unfolding. By 2020, a total of sixteen provinces has already passed gender parity laws requiring that half of the positions in party lists must be filled by women.

Overall, the difussion of gender quotas resulted in a larger presence of women: the number of women in assemblies went from an average of 6.1% in 1990, to an average of 28.9% in 2016 (Barnes and Jones 2018).

This repository provides information of the quota laws adopted in Argentine provinces since 1992. It comprises:

(a) dates of adoption and implementation of the provincial quotas,<br />
(b) requirements of the composition of party lists, and<br />
(c) copies of the provincial laws (available at the '<a href="https://github.com/santiago-alles/prov_quotas/tree/master/legislation">legislation</a>' folder).

Legislation has been compiled from provincial electoral authorities, provincial electoral courts, among others.

Data Availability
------------------

Data can be directly called from the repository using Hadley Wickham's <a href="https://cran.r-project.org/web/packages/readr/readr.pdf" target="_blank">readr</a> package:

<pre><code>require(readr)
url <- 'https://raw.githubusercontent.com/santiago-alles/prov_quotas/master/'
file <- 'ProvQuotas_ARG19922020_V20200925.csv'
read_csv(paste(url, file, sep='/')) -> dat
</code></pre>

Special characters may appear in string variables (e.g., name and last name, party labels, etcetera). Character strings might be converted to <code>UTF-8</code> encoding using <code>iconv</code>:

<pre><code>iconv(x, from = 'latin1', to = 'UTF-8')</code></pre>

Suggested Citation
------------------

When using this dataset, please cite:

<b>Alles</b>, Santiago. 2018. Equilibrar el terreno: Instituciones Electorales e Incorporación de Mujeres en las Legislaturas Provinciales en Argentina. <em>Mujeres en la política: Experiencias nacionales y subnacionales en América Latina</em>, edited by F. Freidenberg, M. Caminotti, B. Muñoz-Pogossian, and T. Došek. Ciudad de México: Instituto Electoral de la Ciudad de México - Universidad Nacional Autónoma de México, pp. 167-192.


