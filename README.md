<?xml version="1.0" encoding="UTF-8"?>
<style xmlns="http://purl.org/net/xbiblio/csl" version="1.0">
  <info>
    <title>ABNT NBR 6023:2018 e 10520:2023</title>
    <id>http://www.citationstyles.org/abnt-nbr-6023-2018</id>
    <link href="http://www.citationstyles.org/abnt-nbr-6023-2018" rel="self"/>
    <author>
      <name>Personalizado</name>
    </author>
    <category citation-format="author-date"/>
    <category field="generic-base"/>
    <updated>2025-03-19T00:00:00Z</updated>
  </info>

  <macro name="author">
    <names variable="author">
      <name and="text" delimiter=", " initialize-with="." name-as-sort-order="first"/>
    </names>
  </macro>

  <macro name="title">
    <text variable="title" font-style="italic"/>
  </macro>

  <macro name="publication">
    <group delimiter=", ">
      <text variable="publisher"/>
      <text variable="publisher-place"/>
    </group>
  </macro>

  <macro name="issued">
    <date variable="issued">
      <date-part name="year"/>
    </date>
  </macro>

  <citation>
    <sort>
      <key variable="author"/>
      <key variable="issued"/>
    </sort>
    <layout prefix="(" suffix=")" delimiter="; ">
      <text macro="author"/>
      <text macro="issued" prefix=", "/>
      <text macro="page" prefix=", p. "/>
    </layout>
  </citation>

  <bibliography>
    <sort>
      <key variable="author"/>
      <key variable="issued"/>
    </sort>
    <layout>
      <group delimiter=". ">
        <text macro="author" suffix="."/>
        <text macro="title" suffix="."/>
        <text macro="publication" suffix=", "/>
        <text macro="issued" suffix="."/>
      </group>
    </layout>
  </bibliography>
</style>
