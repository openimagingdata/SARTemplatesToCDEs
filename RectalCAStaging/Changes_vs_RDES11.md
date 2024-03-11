# Proposed Changes from RDES11 from 2016

- Change 1: rename "RDE70 - Distance of lowest extent of tumor from top of anal sphincter" as "RDE70 - Distance of lowest extent of tumor from top of sphincter complex/anorectal junction"
- Change 2: update "RDE74 - Mucinous tumor"
  - More detailed values (instead of Y/N)
  -     {
          "name": "RDE74 - Mucinous composition",
          "description": "The mucinous composition of the tumor",
          "type": "choice",
          "values": ["No mucin", "Some mucin", "Mostly mucin"]
        }
- Change 3: update "RDE92 - T-category"
  -    {
      "name": "RDE92 - MR-T Category",
      "description": "Magnetic Resonance - T Category of the tumor",
      "type": "valueset",
      "values": [
            "Tx (tumor not seen, post transanal excision/polypectomy)",
            "T1/2 (tumor confined to rectal wall)",
            "T3a (tumor penetrates < 1 mm beyond muscularis propria)",
            "T3b (tumor penetrates 1- 5 mm beyond muscularis propria)",
            "T3c (tumor penetrates >5-15 mm beyond muscularis propria)",
            "T3d (tumor penetrates > 15 mm beyond muscularis propria)",
            "T4a (visible tumor signal thickening and/or nodularity of the anterior peritoneal reflection – may also apply to tumor signal extending laterally along peritoneal reflection)",
            "T4b (tumor invades or adherent to adjacent organs or structures)"
          ]
        }
- Change 4: update "RDE94 - Lower extent relative to puborectalis" and "RDE95 - Most penetrating component"
  - {
      "name": "RDE94 - Low Rectal Tumors - Invasion of Anal Sphincter Complex",
      "description": "Assessment of anal sphincter complex invasion in low rectal tumors",
      "attributes": [
        {
          "name": "Invasion status",
          "description": "Invasion status of the anal sphincter complex",
          "type": "choice",
          "values": ["Absent", "Invades internal sphincter only", "Invades IS and extends into ISS", "Invades IS + ISS + extends into or through external sphincter"]
        },
    {
       "name": "RDE95 - Area of involvement",
       "description": "Area of involvement in the anal canal",
       "type": "choice",
       "values": ["N/A", "Upper anal canal", "Mid anal canal", "Distal anal canal"]
        },
- Change 5: update "RDE97 - Distance-to-MRF information"
  - change value "3 = Not applicable (involving the peritonealized portion of the rectum or T4a)" to "3 = N/A: (tumor at peritonealized portion of the rectum)"
- Change 6: update "RDE98 - Extramural depth of invasion"
  -         {
          "name": "RDE98 - MRF Status",
          "description": "Distance from the tumor margin to the MRF",
          "type": "valueset",
          "values": ["1= Clear (tumor margin >2 mm from MRF)", "2= Threatened (tumor margin within 1-2 mm of MRF)", "3= Involved (tumor margin <1 mm from the MRF)"]
        }
- Change 7: update "RDE99 - Tumor component closer to the MRF"
  -         {
          "name": "RDE99 - Separate tumor deposit, LN or EMVI threat or invasion to MRF",
          "description": "Presence of separate tumor deposit, lymph node, or EMVI threatening or invading the MRF",
          "type": "valueset",
          "values": ["No", "Yes"]
        }
- Change 8: add Tumor Morphology
          {
          "name": "Tumor morphology",
          "description": "The morphology of the tumor",
          "type": "choice",
          "values": ["Polypoid", "Annular", "Partly annular"]
        },
- Change 9: add EMVI
      {
      "name": "EMVI",
      "description": "Extramural Vascular Invasion",
      "attributes": [
        {
          "name": "EMVI status",
          "description": "Presence or absence of EMVI",
          "type": "choice",
          "values": ["No", "Yes"]
        },
- Change 10: Add Tumor Deposits
  {
      "name": "Tumor Deposits",
      "description": "Presence and characteristics of tumor deposits",
      "attributes": [
        {
          "name": "Presence of tumor deposits",
          "description": "Whether tumor deposits are identified",
          "type": "choice",
          "values": ["None identified", "Yes"]
        },
- Change 11: Add Lymph Nodes
      {
      "name": "Lymph Nodes",
      "description": "Assessment of Lymph Nodes",
      "attributes": [
        {
          "name": "Mesorectal/superior rectal lymph nodes and/or tumor deposits",
          "description": "Status of mesorectal/superior rectal lymph nodes and tumor deposits",
          "type": "choice",
          "values": ["N0 (no visible lymph nodes/deposits)",
                     "N+ (short axis ≥ 9 mm)",
                     "N+ (short axis 5 - 8.9 mm AND at least 2 suspicious morphologic criteria)",
                     "N+ (short axis <5 mm AND all 3 suspicious morphologic criteria)",
                     "Nx (indeterminate, all other cases)"]
        },
        {
          "name": "Suspicious extra mesorectal lymph nodes",
          "description": "Presence of suspicious extra mesorectal lymph nodes",
          "type": "choice",
          "values": ["No", "Yes"]
        },
        {
          "name": "Short axis diameter of extra mesorectal lymph nodes",
          "description": "Short axis diameter of suspicious extra mesorectal lymph nodes",
          "type": "numeric",
          "unit": "mm"
        },
          {
          "name": "Location of extra mesorectal lymph nodes",
          "description": "Location of extra mesorectal lymph nodes",
          "type": "valueset",
          "values": ["1= Right internal iliac", "2= Left internal iliac", "3= Right obturator", "4= Left obturator", "5= Right inguinal", "6= Left inguinal", "7= Right common iliac", "8= Left common iliac", "9= Right external iliac", "10= Left external iliac", "11= Right retroperitoneal", "12= Left retroperitoneal"]
        },











