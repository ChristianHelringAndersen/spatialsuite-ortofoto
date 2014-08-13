--------------------
Modul til visning af ortofoto fra Kortforsyningen
-------------------- 

INSTALLATION :

1:   Install�r modulet
1.a: Kopi�r modulet "ortofoto" til sitets moduler, dvs. til "[cbinfo.config.dir]/modules/custom/ortofoto"
1.b: Skriv f�lgende entry i [cbinfo.modules]: <module name="ortofoto" dir="custom/ortofoto" permissionlevel="public"/>

2:   Rediger Profil(er)
2.a: Tilf�j et eller flere af temaerne til profilen.
2.b: Det kan evt. g�res vha. includes af hhv. temagruppe og temaer:

	SpS post 2.6.x :
	
		<include onlychildnodes="true" src="[module:ortofoto.dir]/profiles/includes/themegroups.xml" mustexist="true"/>
        
	Sps pre 2.6.x :	
		
		<include mustexist="false" nodes="/profile/themegroups/*" src="[module:kust.dir]/profiles/profile.xml"/>
	
	SpS post 2.6.x :
	
	<include onlychildnodes="true" src="[module:ortofoto.dir]/profiles/includes/themes.xml" mustexist="true"/>
	
	SpS pre 2.6.x :
	
        <include mustexist="false" nodes="/profile/themes/*" src="[module:kust.dir]/profiles/profile.xml"/>
      

3:	 Tilf�j signatur (s�fremt der �nskes signaturforklaring)

3.a: Billeder i /images kopieres til /resources/symbols/custom/images/

3.b: F�lgende s�ttes ind i symbols5_6.txt:

SYMBOL
    NAME 'ortofoto'
    TYPE PIXMAP
    IMAGE 'custom/images/ortofoto.png'
END


BEM�RKNINGER

Datasource er sat op til ortofoto for HRKS omr�det. S�fremt der �nskes vist for andre omr�der skal disse lag tilf�jes til datasource filen, erstat evt. navnene p� de nye datasources med de eksisterende i tema-filerne. Nedenst�ende er sakset fra Kortforsyningen. Der tages intet ansvar for eventuelle �ndringer og fejl i denne liste, og den vil som udgangspunkt ikke blive opdateret.

Lag
orto_foraar
hrks_2013_10cm
geosjaelland_2013_10cm
geomidt_2013_10cm
geofyn_2013_10cm
hrks_2012_10cm
geosjaelland_2012_10cm
geonord_2012_10cm
viborg_skive_2012_10cm
sydkort_2012_10cm
geofyn_2012_10cm
fyn_2011_10cm
jylland_2011_10cm
jylland_2011_20cm
sjaelland_2011_10cm
bornholm2010_hrks10cm
fyn2010_20cm
fyn2010_10cm
jylland2010_20cm
jylland2010_10cm
sjaelland2010_20cm
sjaelland2010_10cm
sjaelland2010_hrks10cm
jylland2009_20cm
jylland2009_10cm
sjaelland2009_20cm
sjaelland2009_10cm
jylland2008_20cm
jylland2008_10cm
sjaelland2008_10cm
bornholm2007_10cm
jylland2007_20cm
jylland2007_10cm
sjaelland2007_10cm
jylland2006_10cm
jylland2006_20cm
jylland2006_40cm
sjaelland2006_40cm
sjaelland2006_10cm
bornholm2006_40cm
fyn2005_40cm
jylland2005_40cm
jylland2004_40cm

VERSIONSHISTORIK

13-8-2014:	F�rste version

	

