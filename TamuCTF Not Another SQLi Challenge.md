---


---

<h1 id="not-another-sqli-challenge">Not Another SQLi Challenge</h1>
<p>Not Another SQLi Challenge is a challenge for TAMUctf 2019 under the “Secure Coding” section. It’s difficulty is listed as “Easy”, and the question description only includes the link: <a href="http://web1.tamuctf.com">http://web1.tamuctf.com</a></p>
<p>The link takes you to a page with two input fields labeled “NetID” and “Password”. Inputting <strong>admin</strong> into both fields to causes the page to respond with:<br>
Sorry to say, that’s invalid login info!<br>
When entering data with a single quote, the site displays a blank page, suggesting that the input is being parsed literally. I then entered <strong>anything’ OR ‘x’ = ‘x’</strong> because <strong>‘x’ = ‘x’</strong> is always guaranteed to be true. The page then output the flag of “gigem{f4rm3r5_f4rm3r5_w3’r3_4ll_r16h7}!”</p>

