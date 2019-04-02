# Play-Store-Comment-Scrapper

Scrapping data komentar dari playstore, pada kasus ini contoh komentar yang diambil adalah aplikasi bukalapak

- Menggunakan library python Selenium dan beautifulsoup
- terdapat beberapa proses manual yang harus dilakukan

# Contoh Data

<table cellspacing="0" border="0">
	<colgroup span="5" width="64"></colgroup>
	<tr>
		<th style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="left" valign=bottom><font color="#000000">title</font></th>
		<th style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">user_name</font></th>
		<th style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">rating</font></th>
		<th style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">review_date</font></th>
		<th style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">review_text</font></th>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="left" valign=bottom><font color="#000000">Bukalapak-JualBeliOnline</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">uan fadly</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Rated 5 stars out of five stars</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="right" valign=bottom sdval="43530" sdnum="1033;1033;D-MMM-YY"><font color="#000000">6-Mar-19</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">good app</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="left" valign=bottom><font color="#000000">Bukalapak-JualBeliOnline</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">A Google user</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Rated 4 stars out of five stars</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="right" valign=bottom sdval="43530" sdnum="1033;1033;D-MMM-YY"><font color="#000000">6-Mar-19</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">thnks</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="left" valign=bottom><font color="#000000">Bukalapak-JualBeliOnline</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Ricky Oloan</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Rated 1 stars out of five stars</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="right" valign=bottom sdval="43530" sdnum="1033;1033;D-MMM-YY"><font color="#000000">6-Mar-19</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">timernya utk serbu seru ngulang2 terus menerus.....padahal udah waktunya</font></td>
	</tr>
	<tr>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" height="20" align="left" valign=bottom><font color="#000000">Bukalapak-JualBeliOnline</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Ratno Deswara</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">Rated 5 stars out of five stars</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="right" valign=bottom sdval="43530" sdnum="1033;1033;D-MMM-YY"><font color="#000000">6-Mar-19</font></td>
		<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000" align="left" valign=bottom><font color="#000000">lebih praktis</font></td>
	</tr>
</table>

# Visual 

<div class='tableauPlaceholder' id='viz1554213174905' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bu&#47;BukalapakRatePlayStore&#47;BukalapakRate&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BukalapakRatePlayStore&#47;BukalapakRate' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bu&#47;BukalapakRatePlayStore&#47;BukalapakRate&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>                
