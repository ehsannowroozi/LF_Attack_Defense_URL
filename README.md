# Ensemble Trees: A Defense Mechanism Against Label Flipping in Malicious URL Detection

2023-2024 Centre for Secure Information Technologies (CSIT), Queen's University Belfast (QUB), Northern Ireland, United Kingdom

Authors: [Ehsan Nowroozi](https://scholar.google.com/citations?user=C0bNkP8AAAAJ&hl=en) Personal Website: www.enowroozi.com, Email: e.nowroozi@qub.ac.uk

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.

---
#  Introduction:
In the modern digital age, identifying malicious URLs is vital for protecting individuals and systems from online threats. However, because we rely more on Machine Learning (ML) for these tasks, they become vulnerable to covert attacks such as Label Flipping (LF). Such attacks can cause misclassifications, emphasizing the need for built-in defence strategies in ML models. This research delves into backdoor attacks on URL detection via ensemble trees, shedding light on the attackers' motives and the significance of robust defense methods. We introduced a system to spot tainted labels and a defense approach to reveal true labels, aiming to lessen the effects of these attacks. Our tests show that these covert attacks can trick the system, but with our defense, accuracy is restored.


# Steps to Enhance Adversarial Attack Transferability:

1) We started by running an RF model on several pristine datasets to measure its initial performance, creating a benchmark to spot any anomalies in its behavior later.
2) We then subjected the RF models to random LF attacks by introducing varying poison rates in the training data. The results highlighted the RF model's susceptibility as it failed to recognize the attack, though the training accuracy remained within acceptable limits.
3) Lastly, we assessed the KNN method's ability to detect and correct tainted labels. After cleaning these labels, we observed a general improvement in training accuracy across all datasets.

In the attached files related to our paper titled "Defending Against Label Flipping Attacks in Malicious URL Detectors Using Ensemble Trees", you'll find three primary directories:

Random Forest Model in its unattacked state.
Random Label Flipping Attack with adjustable poison rates (NOTE: You can tweak the poison rate in the code as needed).
KNN Defense Strategy against the random label flipping attack.
For implementing the defense strategy, first consult "Check the value of K.py" to determine the appropriate K values. Then, you can run the defense code tailored to your specific tools.


# If you utilize this code, kindly cite the following papers in your *.bib file:

 For the paper titled "An Adversarial Attack Analysis on Malicious Advertisement URL Detection Framework" published in IEEE Transactions on Network and Service Management in June 2023:

##The the paper is available on https://ieeexplore.ieee.org/abstract/document/9964424
##Bib Citation address is: 
  @ARTICLE{9964424,
  author={Nowroozi, Ehsan and Abhishek and Mohammadi, Mohammadreza and Conti, Mauro},
  journal={IEEE Transactions on Network and Service Management}, 
  title={An Adversarial Attack Analysis on Malicious Advertisement URL Detection Framework}, 
  year={2023},
  volume={20},
  number={2},
  pages={1332-1344},
  doi={10.1109/TNSM.2022.3225217}}

