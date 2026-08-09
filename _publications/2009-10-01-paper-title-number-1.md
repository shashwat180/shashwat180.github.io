---
title: "IGZO-Based 2T0C DRAM as an Intrinsic Rowhammer Mitigation: A Device Physics Analysis"
collection: publications
category: manuscripts
#permalink: /publication/2009-10-01-paper-title-number-1
excerpt: "This paper analyzes the two-transistor zero-capacitor (2T0C) DRAM architecture based on amorphous indium-gallium-zinc-oxide (IGZO) thin-film transistors as an intrinsic structural mitigation against Rowhammer, arising not from an explicit security mechanism but from the material properties of IGZO itself."
date: 2026-28-04
#venue: 'Journal 1'
#slidesurl: 'https://academicpages.github.io/files/slides1.pdf'
paperurl: "https://shashwat180.github.io/files/ECE6458_paper.pdf"
#bibtexurl: 'https://academicpages.github.io/files/bibtex1.bib'
#citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

Rowhammer attacks exploit parasitic charge disturbance between adjacent rows in conventional one-transistor one-capacitor (1T1C) DRAM, where the leakage current of silicon access transistors enables sufficient charge injection into victim rows to cause bit flips under repeated aggressor row activations. Despite system-level mitigations such as Target Row Refresh (TRR), Rowhammer vulnerability has persisted and worsened with DRAM scaling, as shrinking cell pitch increases inter-row coupling while silicon transistor leakage remains a fundamental material constraint. This paper analyzes the two-transistor zero-capacitor (2T0C) DRAM architecture based on amorphous indium-gallium-zinc-oxide (IGZO) thin-film transistors as an intrinsic structural mitigation against Rowhammer, arising not from an explicit security mechanism but from the material properties of IGZO itself. Drawing on published device characterization data, we show that IGZO's wide bandgap and ultra-low off-state leakage current reduces the charge disturbance available to an aggressor row by several orders of magnitude compared to silicon-based 1T1C cells at equivalent nodes. We further analyze how the elimination of the storage capacitor in 2T0C cells removes the primary parasitic coupling path exploited in classical Rowhammer, and discuss how the decoupled read and write transistor architecture limits the propagation of disturbance charge to neighboring rows. We contextualize these findings against published Rowhammer threshold measurements across DDR3 through DDR5 and argue that 2T0C IGZO DRAM, if adopted at scale, would render the classical Rowhammer attack physically implausible without requiring any software or firmware mitigation layer. Tradeoffs in write speed, process maturity, and integration with existing memory interfaces are also discussed.
