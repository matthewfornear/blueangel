# smart-mrna-cancer-detector

A synthetic mRNA construct that executes an AND logic gate in human cells:
- Activates only when: **MYC is high**, **ROS is high**, **let-7 is low**
- Expresses GFP as a proof-of-concept payload
- Modular input logic for future therapeutic use

## Project Structure

```
smart-mrna-cancer-detector/
├── README.md                # Overview, logic, usage
├── response_modules/        # Reusable, isolated sensing logic parts
│   ├── let7_response_module.txt     # Degradation logic via miRNA
│   ├── ros_response_module.txt      # Translation logic via ROS gate
│   └── myc_response_module.txt      # Transcription logic via MYC promoter
├── construct/               # Assembled scaffold representing full mRNA design
│   ├── full_mrna_construct.txt      # Final design blueprint, logic stitched
│   ├── full_mrna_sequence.fasta     # FASTA format of mRNA
│   ├── full_dna_sequence.txt        # DNA version
│   └── smart_mrna_construct_genbank.txt # GenBank format
├── payload/                 # Placeholder for gene of interest (e.g., GFP)
│   └── gfp_sequence_placeholder.txt
├── folding/                 # RNA folding and structure predictions
│   ├── smart_mrna_g_mountain.pdf
│   ├── smart_mrna_g_ss.pdf
│   ├── smart_mrna_g_centroid.pdf
│   ├── smart_mrna_g_pp.pdf
│   ├── smart_mrna_g_centroid_pp.pdf
│   ├── smart_mrna_g_pe.pdf
│   └── smart_mrna_g_centroid_pe.pdf
├── output/                  # Output and reports
│   ├── smart_mrna_gfp_logic_construct-sequence.pdf
│   ├── smart_mrna_g_mountain.pdf
│   ├── smart_mrna_g_ss.pdf
│   ├── smart_mrna_g_centroid.pdf
│   ├── smart_mrna_g_pp.pdf
│   ├── smart_mrna_g_centroid_pp.pdf
│   ├── smart_mrna_g_pe.pdf
│   └── smart_mrna_g_centroid_pe.pdf
├── GB/                      # GenBank and plasmid files
│   ├── smart_mrna_gfp_logic_construct.gb
│   ├── pBR322.gb
│   ├── pBR322_EGFR.gb
│   ├── pCMV-VSV-G.gb
│   ├── lentiCRISPR_v2.gb
│   ├── pLKO.1_-_TRC_cloning_ve.gb
│   ├── pMD2.G.gb
│   ├── pSpCas9(BB)-2A-GFP_(PX4.gb
│   ├── pX330-U6-Chimeric_BB-CB.gb
│   ├── pX335-U6-Chimeric_BB-CB.gb
│   ├── psPAX2.gb
│   └── scramble_shRNA.gb
├── documents/               # Patent and documentation
│   ├── Smart_mRNA_Provisional_Patent_Matthew_Fornear_Final.pdf
│   ├── Smart_mRNA_Provisional_Patent_Matthew_Fornear.docx
│   └── Provisional Patent Draft Synthetic.txt
├── patent/                  # Patent text
│   └── smart_mrna_gfp_logic_construct.txt
├── rna_construct_layout.txt # Layout notes
├── logic_signature.txt      # Logic signature
├── potentialtargets.txt     # Potential target list
└── Export of ALL.zip        # Archive of all files
```

## Logic Flow
MYC_HIGH (transcription level)
↓
ROS_HIGH (translation gate)
↓
LET7_LOW (stability gate)
↓
GFP expression

## Files

### /response_modules
- Individual sensor components
- Each file contains RNA logic for a specific signal condition

### /construct
- Assembled scaffold representing full mRNA design

### /payload
- Placeholder for gene of interest (e.g., GFP)

## Usage

1. Read logic in `/construct/full_mrna_construct.txt`
2. Replace GFP with any therapeutic gene in `/payload/`
3. Simulate folding before synthesis
4. Clone into plasmid for MYC-sensitive delivery or use for direct mRNA synthesis

## Dead Man's Switch Licensing

If I, the author and creator of this repository, perish or am otherwise permanently incapacitated, all research, documents, code, designs, and materials contained herein are immediately and irrevocably released into the public domain. Anyone is free to use, modify, distribute, or build upon this work for any purpose, without restriction, in perpetuity.

This clause overrides any other licensing or usage restrictions that may otherwise apply.

