# [Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python Code]

With the development of cognitive radio technology (CRT) in wireless communication networks, deep learning (DL) plays a significant role in enhancing spectrum efficiency. However, supervised learning methods require large amounts of labeled data and are costly in terms of labor. Therefore, there is an increasing need for technologies that learn robust representations from unlabeled data in CRT applications. Although recent advances in DL have propelled the application of self-supervised learning (SSL) through time-domain contrastive methods in CRT, these methods often neglect temporal-frequency features, making it challenging to extract advanced spectral representations. To address this, this paper proposes a generative SSL framework suitable for CRT. Firstly, masked autoencoders (MAE) are used for pretraining in both time and frequency domains to extract features through reconstructing masked spectral graphs; secondly, for restoring spectral graphs in extreme wireless environments, mutual information maximization (MIM) is employed to extract high-level spectral information obscured by noise; furthermore, an attention-based channel-spectrum fusion module is designed to automatically extract and fuse features from both the channel and spectral domains. Multiple downstream tasks evaluation on four public datasets demonstrates that this framework significantly outperforms existing methods across various tasks.
Introduction Research background and challenges With the proliferation of wireless devices and the scarcity of spectrum resources, the management and optimization of limited wireless network resources face significant challenges. Cognitive radio technology (CRT) becomes an effective solution for spectrum sharing optimization and improving communication quality by real-time monitoring, analysis, and exploitation of radio spectrum. In key tasks of CRT such as radio signal classification, signal denoising, and partial signal loss restoration, machine learning (ML) and deep learning (DL) can identify modulation schemes and improve spectrum allocation efficiency. However, traditional ML methods are affected by device internal noise and interference sources, making it difficult to accurately recognize radio signals. While DL methods can learn complex nonlinear high-dimensional features from data, supervised learning (SL) heavily relies on large amounts of labeled data, which is costly in wireless communication scenarios and limits practical deployment, especially in scenarios with scarce labeled data.
The development and limitations of self-supervised learning (SSL) as a solution to the problem of limited labeled data. SSL learns feature representations through pre-training tasks, which can be transferred to downstream tasks. The existing SSL methods in CRT applications have the following limitations:
Downstream tasks are limited to single signal classification
Comparative SSL methods (such as MoCo, SimCLR) learn features by comparing positive and negative samples, but only support signal classification (RSC), unable to handle multiple tasks simultaneously.
Lack of effective extraction of time-frequency domain features
Generative SSL methods (such as MAE) focus on the latent representation of data, but the basic Transformer model lacks understanding of signal modulation information and channel characteristics, making it difficult to extract advanced spectral features from radio signals.
Feature extraction challenges under extreme conditions
In extreme scenarios such as low SNR, high data loss rate, etc., generative SSL models struggle to converge due to noise and distortion, unable to extract advanced spectral information obscured by noise.
This paper contributes to the design of an attention channel - spectrum fusion Transformer based MAE (ACSF-TMAE) framework, with main contributions including:
Integrating the time-frequency characteristics of radio signals into the learning process to capture long-distance spectral feature relationships, suitable for multiple downstream tasks.
Designing an Attention Channel - Spectrum Fusion (AC-SF) module to automatically extract features from regions with concentrated spectral energy, enhancing the network's understanding of important latent features.
Using weakly enhanced latent features to guide the reconstruction of strongly enhanced features, extracting advanced spectral information in noise through MIM, providing a theoretical basis for reconstruction.
Experiments on four datasets show that even with only 10% of the data trained, this method significantly outperforms other SSL and SL methods in terms of classification accuracy and robustness, performing well in denoising and missing data recovery tasks.
Article illustration
Conclusion: This paper explores the application of generative SSL framework in CRT (Time-Frequency domain), aiming to address the lack of flexibility and generality in existing SSL methods. The proposed ACSF-TMAE enhances denoising, classification, and signal completion tasks by better understanding global and local features of spectrum graphs through pre-training. Leveraging MIM (Mutual Information Maximization) theory, it guides the network to extract long-range spectral feature relationships obscured by noise under low SNR conditions, thereby strengthening the ability to extract advanced spectral information. An attention fusion mechanism is designed to address the issue of uneven energy distribution in spectrum graphs, improving the network's understanding of both spectral and channel domain latent features. Experimental results show that this framework can still improve accuracy and generalization performance using only data with SNR≥6 dB for pre-training, and supports a wider range of downstream tasks. Future research hopes to inspire researchers to explore the widespread applications of generative SSL models in CRT.
End

## Images

![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](01.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](02.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](03.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](04.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](05.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](06.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](07.jpg)
![[Modulation Identification] Cognitive Radio Generative Self-Supervised Framework Based on Time-Frequency Features and Attention Fusion [with Python code]](08.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
