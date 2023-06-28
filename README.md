<p align="center">
  <a href="https://www.casd.eu">
  <img src="/logos/casd_logo.png" alt="logo casd" width="500">
  </a>
</p>

These are the slides used to present CASD's meeting paper for [2023 UNECE expert meeting on statistical data confidentiality](https://unece.org/statistics/events/SDC2023).
You can find the list of all speakers and abstracts [here](https://indico.un.org/event/1002843/).

---

### Abstract

CASD is a public organization which can be likened to a research data center: it hosts a large amount of highly detailed data from various administrations (tax data, health data, industrial data, etc.). These data pertain both to firms and people and are protected by different legal confidentiality regulations: medical secrecy, statistical secrecy, business secrecy and so on.
The aim of CASD is to make such data available for research purposes, duly authorized by the data producers. CASD developed a specific remote access system which enables the researcher to visualize data, to interactively process any calculations for their research, with a wide range of scientific and data analysis software tools (SAS, R, Python...) and technologies (Spark, Pandas..) at their disposal. Scientific article editing software are also installed in the virtual environment.
At the end of these processes, final outputs for publication must be anonymized. The enrolment and training sessions, which users must complete before accessing the data, include rules for output anonymization. The CASD data platform enforces a strong security policy, which includes an output checking procedure: even if each researcher is accountable for their research work, especially when it comes to the compliance of the outputs retrieved from their virtual research environment with GDPR or various confidentiality regulations, additional safeguards are in place. In particular, most of the outputs are manually controlled by CASD staff according to the rules data producers have established for this purpose. However, some projects hosted by the CASD infrastructure can ask for "automatic outputs" where manual checking is not systematic. This requires the authorization of every data producer involved. Usually, some outputs are forbidden in order to prevent massive disclosure (size and number of outputs are limited, encrypted files are forbidden). Manual checks are conducted randomly for other outputs, by CASD staff or by producers directly.
In order to make the system more efficient, CASD has developed a new tool, based on a Deep Neural Network (DNN) model. The model was trained using approximately 11k previous results of manual output checks: ok or refused, and the reason for elements rejected. A list of controls (the details of which are confidential), for metadata elements (elements of context) as well as for content of files, is implemented for each output. It is important to point out that the algorithm is able to open more than fifty file format types (csv, sas...) and to check their content, especially for detecting individual data patterns. Once all this has been carried out, the algorithm provides a "risk score": if the score is too high, the output is manually checked by a CASD employee. The final check result is used to train the DNN model to continuously improve its accuracy. First training runs of the model are based on manual checks, then continuously increased with semi-automatic checks.

This presentation aims to explain how this system works.

---
