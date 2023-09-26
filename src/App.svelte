<script lang="ts">
  import Textfield from "@smui/textfield";
  import SegmentedButton, { Segment } from '@smui/segmented-button';
  import { Label } from '@smui/common';

  const choices = ["moški", "ženski", "srednji"];

  let pritozbeni_subjekt = "SIOL";
  let sklanjatev_rodilnik = "SIOL-a";
  let sklanjatev_tozilnik = "SIOL";
  let sklanjatev_mestnik = "SIOL-u";
  let alternativa = "T-2";
  let storitve = "vašega interneta";
  let troubleshooting = "resetirat modem";
  let nedelujoci_subjekt = "modem";
  let zacetna_pritozba = "najbolj beden, najbolj smrdljiv, najbolj kretenski internetni ponudnik v Sloveniji";
  let spol = "moški";
  let spol_alt = "moški";
  let spol_skupina = "moški";
  let skupina = "ponudniki interneta";
</script>

<main>
  <h1>SIOL pritožba generator</h1>

  <h2>Spremenljivke</h2>

  <Textfield bind:value={pritozbeni_subjekt} label="Pritožbeni subjekt (v imenovalniku)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={sklanjatev_rodilnik} label="Pritožbeni subjekt (v rodilniku, koga/česa)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={sklanjatev_tozilnik} label="Pritožbeni subjekt (v tožilniku, koga/kaj)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={sklanjatev_mestnik} label="Pritožbeni subjekt (v mestniku, o kom/o čem)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={zacetna_pritozba} label="Začetno dejstvo (je najbolj beden, najbolj smrdljiv, najbolj kretenski internetni ponudnik v Sloveniji)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={alternativa} label="Ne tako dobra alternativa trenutnemu pritožbenemu subjektu (Če ne bo T-2 spremenil stvari na slov. trgu...)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={storitve} label="Storitev (o kvaliteti vašega interneta)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={skupina} label="Skupina (da so usi ponudniki interneta v Sloveniji poslovni partnerji od SIOL-a)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={troubleshooting} label="Iskanje težav (a ste že probal resetirat modem)" style="width: 100%" helperLine$style="width: 100%;" />
  <Textfield bind:value={nedelujoci_subjekt} label="Nedelujoči subjekt (koga/kaj mu jebemo v pičko (pičko materino i ta modem))" style="width: 100%" helperLine$style="width: 100%;" />

  <p/>
  Spol pritožbenega subjekta ({pritozbeni_subjekt}:
  <br>
  <SegmentedButton segments={choices} let:segment singleSelect bind:selected={spol}>
    <!-- Note: the `segment` property is required! -->
    <Segment {segment}>
      <Label>{segment}</Label>
    </Segment>
  </SegmentedButton>

  <p/>

  Spol alternative ({alternativa}):
  <br>
  <SegmentedButton segments={choices} let:segment singleSelect bind:selected={spol_alt}>
    <!-- Note: the `segment` property is required! -->
    <Segment {segment}>
      <Label>{segment}</Label>
    </Segment>
  </SegmentedButton>

  <p/>

  Spol skupine ({skupina}):
  <br>
  <SegmentedButton segments={choices} let:segment singleSelect bind:selected={spol_skupina}>
    <!-- Note: the `segment` property is required! -->
    <Segment {segment}>
      <Label>{segment}</Label>
    </Segment>
  </SegmentedButton>

  <h2>{pritozbeni_subjekt} pritožba</h2>

  <p/>

  V naslednjih dveh minutah bom povedal svoje subjektivno mnenje o {sklanjatev_mestnik},
  <br>
  zatorej me ne prekinjajte, in si ne mislite da vam to govorim kot grožnjo,
  <br>
  temveč vzemite to kot <b>OSEBNO</b>, <b>SUBJEKTIVNO</b> mnenje o {sklanjatev_mestnik}.
  <br>
  No pa začnimo.

  <p/>

  {pritozbeni_subjekt} je {zacetna_pritozba}.
  <br>
  <i>tišina</i>
  <br>
  Že dejstvo, da vsakič, k mi {pritozbeni_subjekt} ne dela,
  <br>
  moram poklicat na vašo po-FUKANO modro številko, k si jo lahko tut zarinete u <b>RT</b> baj d vej,
  <br>
  moram čakat eno po-FUKANO uro, da dobim enga kRRRRETENA na telefon.
  <br>
  K mi pol reče "Ja gospod, a ste že probal {troubleshooting}?"
  <br>
  Ma mrš u <b>PIČKO MATERINO I TA {nedelujoci_subjekt.toUpperCase()} DA TI JEBEM MATER U PIČKO</b>
  <br>
  A ti je jasn?
  <br>
  Jebem ti mater nesposobno
  <br>
  Pa kere mongloide pofukane date tja na telefon
  <br>
  Prokleti kreteni neumni

  <p/>

  Že TO kaže o vaši <b>MALOMARNOSTI</b> do nas uporabnikov,
  <br>
  in bi mogl <b>RESNO</b> razmislt o KVAliteti {storitve},
  <br>
  ne pa o KVANtiteti, da vam jebem mater u pičko.
  <br>
  Nimate nobenih informacj,
  <br>
  zmer k pokličm rečete: "UH, Ja ne vemo klele gospod proti k um ja um.
  <br>
  Klele k gre um proti Nemčiji se je neki ustavl mal-",
  <br>
  <b>MA MRŠ U PIČKO MATER TI JEBEM MATER U PIZDO</b>
  <br>
  Poprav to zdele takoj
  <br>
  Po pa rčte "Ja, bomo dal naprej gospod uh, pa bom vm pol povedu kva se je zgod- Ja uh bom dau naprej ane?"
  <br>
  <b>PA KAJ BOŠ DAL NAPREJ, BOŠ DOU KURAC SEB U RT</b>
  <br>
  <b>PIZDA TI MATRNA GNILA</b>

  <p/>

  To je blo moje mišljenje.
  <br>
  Zdaj pa pozor!
  <br>
  Js mislm, da bi usi mogl preklicat {sklanjatev_tozilnik}
  <br>
  In jt na drug ponudnik interneta
  <br>
  Ampak kle pa nastane en <b>poFUKAN, MEJHN, zajeben u PIĆKU problem</b>,
  <br>
  In <b>TO JE</b>
  <br>
  Da so {#if spol_skupina === "moški"}usi{:else if spol_skupina === "ženski"}use{:else}usa{/if} {skupina} v Sloveniji {#if spol_skupina === "moški"}poslovni partnerji{:else if spol_skupina === "ženski"}poslovne partnerice{:else}poslovni partnerji{/if} od {sklanjatev_rodilnik}.
  <br>
  KAJ PA TO POMEN?
  <br>
  <b>DA GRE <i>VSE PREK {sklanjatev_rodilnik.toUpperCase()} PIZDA TI MATRNA GNILA</i>,</b>
  <br>
  <b>MAMO TI JEBEM U <b>PIČKO</b> i {sklanjatev_tozilnik} da ti jebem.</b>
  <br>
  Kretensko.
  <br>
  Js ne mislm plačvt 7 evri na mesec,
  <br>
  za eno pofukan švabo tmle čez stene strela
  <br>
  <b>DA MU JEBEM MATER</b>
  <br>
  K ve da mam več kil od nega
  <br>
  A ti je jasno?
  <br>
  Da ti jebem.
  <br>
  Gnilo.
  <br>
  Pičko.

  <p/>

  Skratka ...
  <br>
  Če ne bo {alternativa} mau {#if spol_alt === "moški"}spremenu{:else if spol_alt === "ženski"}spremenila{:else}spremenilo{/if} stvari na slovenskem trgu,
  <br>
  pol bomo šli in bomo zažgal {#if spol === "moški"}ta{:else if spol === "ženski"}to{:else}to{/if} <b>{#if spol === "moški"}poFUKAN{:else if spol === "ženski"}poFUKANO{:else}poFUKANO{/if} {sklanjatev_tozilnik}!</b>
  <br>
  Ker mi gre na [?]!
  <br>
  To je blo use.
  <br>
  Hvala.
</main>
