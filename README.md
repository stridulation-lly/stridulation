**Stridulation - Ant Acoustic Communication Research Dataset**

***Project Overview***

This repository is a multimodal dataset for ant stridulation behavior research, designed for analyzing sound signal characteristics across different castes and behavioral contexts. The dataset contains high-resolution audio recordings, spectrogram visualizations, and video examples, providing foundational data for studies in insect acoustic communication, social insect behavior, and bioacoustics.

1.Caste-Specific Datasets

Folder	Description	Sample Features

github.queen/	Queen stridulation data	Attack behavior, trap situations, and example videos

github.male/	Male ant stridulation data	Aggressive encounters, trap contexts with spectrograms

github.worker/	Worker stridulation data	Attack behavior, trap situations (samples 1-30, 31-54), responses to queen stridulation

github.gyne/	Virgin queen (gyne) data	Sound behavior of unmated reproductives

github.dealate_gyne/	Dealated queen data	Acoustic characteristics of post-mating, de-winged individuals


2.Behavioral Category Folders

github.aggressive/ - Recordings related to aggressive behavior

github.submissive/ - Submissive/yielding behavior recordings

github.stop_fight/ - Recordings from conflict de-escalation situations

github.miss_attack/ - Recordings from failed attack attempts

github.playback/ - Sound playback experiment data


 3.Metadata File

github.xlsx - Experimental metadata table (~19.7KB), containing structured information including sample IDs, experimental conditions, timestamps, and other parameters

Data Format Specifications
Audio Data

    Format: WAV/MP4 (audio embedded in video)
    Sampling Rate: Standard configuration based on experimental equipment
    Bit Depth: 16-bit or 24-bit

Visualization Files

    Spectrograms (.png): Time-frequency representations of sound signals
        Examples: male_attack.png, worker_trap.png, queen_attack.png
        Resolution: ~700-800KB per file

Video Examples

    Format: MP4
    Purpose: Provide visual context for sound production
    File Size: 11MB - 22MB
    Includes:
        worker_attack_example.mp4
        male_trap_example.mp4
        queen_attack_example.mp4
        on_gyne_stridulation_example.mp4 (worker response to queen stridulation)

Research Background
Stridulation is the production of sound signals by rubbing specific body parts together (such as abdominal segments or wings). In ants, this acoustic communication is closely associated with:

    Alarm Signals: Emitted when encountering predators or competitors
    Distress Signals: Used to attract nestmate rescue when trapped
    Attack Modulation: Regulating the intensity of intraspecific conflict
    Caste Recognition: Distinct acoustic signatures across castes (workers, queens, males)

This dataset specifically focuses on acoustic differences between trap situations and attack contexts, providing empirical evidence for understanding the evolution of ant emergency communication systems.
Usage Guide
Data Access
bash
复制

# Clone the full repository
git clone https://github.com/stridulation-lly/stridulation.git

# Navigate to specific caste data
cd stridulation/github.worker/
ls github.worker_trap\(1-30\)/

Recommended Analysis Workflows

    Audio Processing: Use Python's librosa or MATLAB for spectrogram analysis
    Statistical Comparison: Compare acoustic parameters (dominant frequency, pulse interval, duration) across castes and behavioral contexts (attack vs. trap)
    Machine Learning: Train caste classifiers or behavior recognition models using spectrogram images

Citation
If you use this dataset, please cite:
复制

Stridulation Dataset: Multi-caste acoustic communication in ants
Repository: https://github.com/stridulation-lly/stridulation
Contact: stridulation-lly (GitHub)

License and Usage
This project is publicly available for academic research and follows standard open-source GitHub licensing. Users should adhere to academic integrity principles and acknowledge the data source in published work.
Contact

Issues: Submit data questions or technical inquiries via GitHub Issues
Maintainer: lliangyu2023@lzu.edu.cn
