# EEG-Database

データベースは, 被験者の情報と聴かせた音楽の情報が記録された「ExperimentInformation」フォルダ, 感性評価値と前処理前の脳波データが記録された「RawData」フォルダ, 前処
理後の脳波データが記録された「PreprocessedData」フォルダから構成されている.

「ExperimentInformation」フォルダの「MusicInformation.xlsx」には被験者に聴かせた音楽の情報が記録されている。本実験での通し番号と, それに対応するDEAPデータセットの音楽番号と感情分類（1:HVHA, 2:LVHA, 3:HVLA, 4:LVLA）が記録されている. 
「SubjectsInformation.xlsx」には被験者番号とそれに対応する性別（M: 男性, F:女性）, 国籍（J:日本人, C:中国人）が記録されている. 

「RawData」フォルダは直下に「s（被験者番号）」フォルダが並んでいて, それぞれの被
験者のデータにアクセスできる. それぞれのフォルダは「CSV」フォルダと「EDF」フォ
ルダと「Label.xlsx」ファイルから構成されている.

「CSV」フォルダでは各曲を聴いた際の被験者の脳波データが, 「（曲番号）~ .csv」とい
うファイル名で CSV 形式で保存されている. 32 チャネルを 128 Hz で測定した際の振幅
（μV）が記録されている. 「EDF」フォルダも同様に, EDF 形式で脳波データが記録され
ている. 「Label.xlsx」ファイルでは, 被験者の国籍, 性別, 各曲に対するその被験者の感性
評価値が記録されている

「PreprocessedData」でも同様に, 直下に「S（被験者番号）.fif」フォルダが並んでいて,
それぞれの被験者の前処理後のデータが FIF 形式で記録されている.


The database consists of an "ExperimentInformation" folder in which the information on the subjects and the music they listened to are recorded, a "RawData" folder in which the sensory evaluation values and EEG data before preprocessing are recorded, and a "PreprocessedData" folder in which the EEG data after preprocessing are recorded.
The "PreprocessedData" folder contains the EEG data after the preprocessing.

MusicInformation.xlsx" in the "ExperimentInformation" folder contains information on the music played to the subjects. The serial number of the music in this experiment, the music number of the corresponding DEAP dataset, and the emotion classification (1:HVHA, 2:LVHA, 3:HVLA, 4:LVLA) are recorded in this folder. 
SubjectsInformation.xlsx" contains subject numbers and their corresponding gender (M: Male, F: Female) and nationality (J: Japanese, C: Chinese). 

The "RawData" folder has a "s (subject number)" folder directly under it, and each subject's data can be accessed.
The "RawData" folder has "s (subject number)" folders directly under it, and you can access the data of each subject. Each folder consists of a "CSV" folder, an "EDF" folder, and a "Label.
Each folder consists of a "CSV" folder, an "EDF" folder, and a "Label.xlsx" file.

In the "CSV" folder, the subject's EEG data for each song are stored in CSV format with the file name "(song number) ~ .csv".
In the "CSV" folder, the subjects' EEG data are stored in CSV format under the file name "(song number) ~ .csv". The amplitude (μV) of 32 channels measured at 128 Hz is recorded.
(μV) of 32 channels measured at 128 Hz are recorded. Similarly, the "EDF" folder records EEG data in EDF format.
The "EDF" folder also contains EEG data in EDF format. The "Label.xlsx" file records the subject's nationality, gender, and the subject's sensitivity
evaluation values for each song.

Similarly, in the "PreprocessedData" folder, there is a "S (subject number).fif" folder directly below the "Label.xlsx" file,
The preprocessed data of each subject is recorded in FIF format.
