# Prüfung Organisation

Standardprüfung ilivalidator. Externe Referenzen werden nicht geprüft. Obwohl die Daten (`gep.xtf`) eine Referenz aufweisen, die ins Leere zeigt, wird keine Fehler gemeldet:

```
java -jar ilivalidator.jar gep.xtf
```

Output:

```
Info: ilivalidator-1.11.10-61c230a3331fd24f2c1dc841ee9519e191915440
Info: ili2c-5.2.2-c48675a2ecb4cf824bcbdcaa76abfdb10bea327e
Info: iox-ili-1.21.6-4c681c10b36fc582a611709d0ee9bf426177876f
Info: User <stefan>
Info: Start date 2021-08-03 18:31
Info: maxMemory 6291456 KB
Info: dataFile <gep.xtf>
Info: pluginFolder </Users/stefan/apps/ilivalidator-1.11.10/plugins>
Info: modeldir <%ITF_DIR;http://models.interlis.ch/;%JAR_DIR/ilimodels>
Info: lookup model <Units> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <Base_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <SIA405_Base_Abwasser_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <VSADSSMINI_2020_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Units-20120220.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Base_d-20181005.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/SIA405_Base_Abwasser-20201103.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/VSADSSMINI_2020_2_d_LV95-20201209.ili>
Info: validate data...
Info: assume unknown external objects
Info: first validation pass...
Info: second validation pass...
Info: validate unique constraint VSADSSMINI_2020_LV95.VSADSSMini.Knoten.Constraint1...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_vonAssoc.Leitung_Knoten_vonAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_TextAssoc.Text...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Bauwerkskomponente_Notenlastung_EinleitstelleAssoc.Bauwerkskomponente_Notenlastung_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_geplantAssoc.Teileinzugsgebiet_Knoten_RW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_geplantAssoc.Teileinzugsgebiet_Knoten_SW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_PAA_KnotenAssoc.SK_PAA_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_KnotenAssoc.Ueberlauf_Foerderaggregat_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlauf_EinleitstelleAssoc.SK_Regenueberlauf_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Massnahme_KnotenAssoc.Massnahme_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_IstAssoc.Teileinzugsgebiet_Knoten_RW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_IstAssoc.Teileinzugsgebiet_Knoten_SW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Trennbauwerk_PrimaerrichtungAssoc.SK_Trennbauwerk_PrimaerrichtungAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_Knoten_nachAssoc.Ueberlauf_Foerderaggregat_Knoten_nachAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlaufbecken_EinleitstelleAssoc.SK_Regenueberlaufbecken_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_nachAssoc.Leitung_Knoten_nachAssocRef...
Info: gep.xtf: VSADSSMINI_2020_LV95.VSADSSMini BID=VSADSSMINI_2020_LV95.VSADSSMini
Info:       1 objects in CLASS VSADSSMINI_2020_LV95.VSADSSMini.Knoten
Info: ...validation done
```

Mit der Option `--allObjectsAccessible` wird ilivalidator mitgeteilt, dass alle Objekte vorhanden sind und die externe Referenz geprüft werden kann:

```
java -jar ilivalidator.jar --allObjectsAccessible gep.xtf
```

Es werden jetzt Fehler gemeldet. Siehe z.B. `Error: line 13: VSADSSMINI_2020_LV95.VSADSSMini.Knoten: tid deg5mQXX20001001: No object found with OID deg5mQXX20000001.`. 

```
Info: ilivalidator-1.11.10-61c230a3331fd24f2c1dc841ee9519e191915440
Info: ili2c-5.2.2-c48675a2ecb4cf824bcbdcaa76abfdb10bea327e
Info: iox-ili-1.21.6-4c681c10b36fc582a611709d0ee9bf426177876f
Info: User <stefan>
Info: Start date 2021-08-03 18:34
Info: maxMemory 6291456 KB
Info: dataFile <gep.xtf>
Info: pluginFolder </Users/stefan/apps/ilivalidator-1.11.10/plugins>
Info: modeldir <%ITF_DIR;http://models.interlis.ch/;%JAR_DIR/ilimodels>
Info: lookup model <Units> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <Base_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <SIA405_Base_Abwasser_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <VSADSSMINI_2020_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Units-20120220.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Base_d-20181005.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/SIA405_Base_Abwasser-20201103.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/VSADSSMINI_2020_2_d_LV95-20201209.ili>
Info: validate data...
Info: first validation pass...
Info: second validation pass...
Info: validate unique constraint VSADSSMINI_2020_LV95.VSADSSMini.Knoten.Constraint1...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Error: line 13: VSADSSMINI_2020_LV95.VSADSSMini.Knoten: tid deg5mQXX20001001: No object found with OID deg5mQXX20000001.
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Error: line 13: VSADSSMINI_2020_LV95.VSADSSMini.Knoten: tid deg5mQXX20001001: No object found with OID deg5mQXX20000001.
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Error: line 13: VSADSSMINI_2020_LV95.VSADSSMini.Knoten: tid deg5mQXX20001001: No object found with OID deg5mQXX20000001.
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Error: line 13: VSADSSMINI_2020_LV95.VSADSSMini.Knoten: tid deg5mQXX20001001: No object found with OID deg5mQXX20000001.
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_vonAssoc.Leitung_Knoten_vonAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_TextAssoc.Text...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Bauwerkskomponente_Notenlastung_EinleitstelleAssoc.Bauwerkskomponente_Notenlastung_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_geplantAssoc.Teileinzugsgebiet_Knoten_RW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_geplantAssoc.Teileinzugsgebiet_Knoten_SW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_PAA_KnotenAssoc.SK_PAA_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_KnotenAssoc.Ueberlauf_Foerderaggregat_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlauf_EinleitstelleAssoc.SK_Regenueberlauf_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Massnahme_KnotenAssoc.Massnahme_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_IstAssoc.Teileinzugsgebiet_Knoten_RW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_IstAssoc.Teileinzugsgebiet_Knoten_SW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Trennbauwerk_PrimaerrichtungAssoc.SK_Trennbauwerk_PrimaerrichtungAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_Knoten_nachAssoc.Ueberlauf_Foerderaggregat_Knoten_nachAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlaufbecken_EinleitstelleAssoc.SK_Regenueberlaufbecken_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_nachAssoc.Leitung_Knoten_nachAssocRef...
Info: gep.xtf: VSADSSMINI_2020_LV95.VSADSSMini BID=VSADSSMINI_2020_LV95.VSADSSMini
Info:       1 objects in CLASS VSADSSMINI_2020_LV95.VSADSSMini.Knoten
Info: ...validation failed
```

Damit die Prüfung validiert, müssen die Organisationen mitvalidiert werden:

```
java -jar ilivalidator.jar --allObjectsAccessible ipw_organisationen.xtf gep.xtf
```

Es werden keine Fehler mehr gemeldet:

```
Info: ilivalidator-1.11.10-61c230a3331fd24f2c1dc841ee9519e191915440
Info: ili2c-5.2.2-c48675a2ecb4cf824bcbdcaa76abfdb10bea327e
Info: iox-ili-1.21.6-4c681c10b36fc582a611709d0ee9bf426177876f
Info: User <stefan>
Info: Start date 2021-08-03 18:37
Info: maxMemory 6291456 KB
Info: dataFile <ipw_organisationen.xtf>
Info: dataFile <gep.xtf>
Info: pluginFolder </Users/stefan/apps/ilivalidator-1.11.10/plugins>
Info: modeldir <%ITF_DIR;http://models.interlis.ch/;%JAR_DIR/ilimodels>
Info: lookup model <SIA405_Base_Abwasser_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <Units> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <Base_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: lookup model <VSADSSMINI_2020_LV95> 2.3 in repository </Users/stefan/sources/afu_ipw_interlis_cookbook/02/>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Units-20120220.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/Base_d-20181005.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/SIA405_Base_Abwasser-20201103.ili>
Info: ilifile </Users/stefan/sources/afu_ipw_interlis_cookbook/02/VSADSSMINI_2020_2_d_LV95-20201209.ili>
Info: validate data...
Info: first validation pass...
Info: first validation pass...
Info: second validation pass...
Info: validate unique constraint SIA405_Base_Abwasser_LV95.Administration.Organisation.Constraint1...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.Knoten_EigentuemerAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_BetreiberAssoc.Leitung_BetreiberAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Massnahme_TraegerschaftAssoc.Massnahme_TraegerschaftAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Massnahme_Verantwortlich_AusloesungAssoc.Massnahme_Verantwortlich_AusloesungAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.VSA_BaseClass_DatenherrAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.VSA_BaseClass_DatenlieferantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Einleitstelle_Ausfuehrende_FirmaAssoc.SK_Einleitstelle_Ausfuehrende_FirmaAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.Knoten_BetreiberAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_StandortgemeindeAssoc.SK_StandortgemeindeAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_EigentuemerAssoc.Leitung_EigentuemerAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_BueroAssoc.SK_BueroAssocRef...
Info: validate unique constraint VSADSSMINI_2020_LV95.VSADSSMini.Knoten.Constraint1...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Info: validate target of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenherrAssoc.DatenherrRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.DatenlieferantAssoc.DatenlieferantRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_vonAssoc.Leitung_Knoten_vonAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_TextAssoc.Text...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Bauwerkskomponente_Notenlastung_EinleitstelleAssoc.Bauwerkskomponente_Notenlastung_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_geplantAssoc.Teileinzugsgebiet_Knoten_RW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_geplantAssoc.Teileinzugsgebiet_Knoten_SW_geplantAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_PAA_KnotenAssoc.SK_PAA_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_KnotenAssoc.Ueberlauf_Foerderaggregat_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_EigentuemerAssoc.EigentuemerRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlauf_EinleitstelleAssoc.SK_Regenueberlauf_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Massnahme_KnotenAssoc.Massnahme_KnotenAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_RW_IstAssoc.Teileinzugsgebiet_Knoten_RW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Teileinzugsgebiet_Knoten_SW_IstAssoc.Teileinzugsgebiet_Knoten_SW_IstAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Knoten_BetreiberAssoc.BetreiberRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Trennbauwerk_PrimaerrichtungAssoc.SK_Trennbauwerk_PrimaerrichtungAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Ueberlauf_Foerderaggregat_Knoten_nachAssoc.Ueberlauf_Foerderaggregat_Knoten_nachAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.SK_Regenueberlaufbecken_EinleitstelleAssoc.SK_Regenueberlaufbecken_EinleitstelleAssocRef...
Info: validate multiplicity of role VSADSSMINI_2020_LV95.VSADSSMini.Leitung_Knoten_nachAssoc.Leitung_Knoten_nachAssocRef...
Info: gep.xtf: VSADSSMINI_2020_LV95.VSADSSMini BID=VSADSSMINI_2020_LV95.VSADSSMini
Info:       1 objects in CLASS VSADSSMINI_2020_LV95.VSADSSMini.Knoten
Info: ipw_organisationen.xtf: SIA405_Base_Abwasser_LV95.Administration BID=Basket1
Info:       1 objects in CLASS SIA405_Base_Abwasser_LV95.Administration.Organisation
Info: ...validation done
```