# Week 2

Discussion:
- The students presented a few slides explaining what they learnt from the papers.
- We discussed more in depth the project goals and the physics scope of the project.
- We will explore the ATLAS MC simulations to try to replicate the calibration strategy from ATLAS.
- The students will have to familiarise with the ATLAS software infrastructure.

Outcomes:



## Code instructions:

### Connect to LxPlus.

From your computer terminal you have to do:
```
ssh <username>@lxplus.cern.ch
```

Then enter your password and the 2nd factor authentication code.

You will land in your AFS working space: `/afs/cern.ch/user/d/YOUR_USERNAME`. This is generally used for storing your code.
The `LxPlus` machines use the Linux OS kernel and you can use your [favourite command line commands](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview).

### Storing your datasets/results.

Data and results should be stored in your `EOS` workspace: `/eos/user/d/YOUR_USERNAME`. You can also acces this space from [Cernbox](https://cernbox.cern.ch/).

To go from `AFS` to `EOS` just to:
```
cd /eos/user/d/YOUR_USERNAME
```

### Setup the ATLAS environment and download your first dataaset.

To setup the ATLAS environment we do:
```
setupATLAS
```

This will print some information on your screen related to the additional ATLAS tools you can setup. The first tool we will use is called `rucio`, it allows us to download ATLAS MC simualtions and real data.

To setup rucio, you have to do:
```
lsetup rucio
```

Before we can start downloading data, we have to authenticate in the LHC Computing Grid!

### Authenticate in the LHC Computing Grid

We first need to generate a certificate, following [these instructions](https://atlassoftwaredocs.web.cern.ch/analysis-software/ASWTutorial/basicSetup/grid_cert/#request-a-certificate).

Then we have to install that certificate in our `LxPlus` space, following [these instructions](https://atlassoftwaredocs.web.cern.ch/analysis-software/ASWTutorial/basicSetup/grid_setup/#install-certificate-on-lxplus-or-a-tier-3).

Once this is completed, we authenticate:
```
voms-proxy-init -voms atlas
```

Now we can use `rucio`!


### Download your first MC sample.

Go to your `EOS` workspace and download the ttbar di-lepton sample:
```
cd /eos/user/d/YOUR_USERNAME
mkdir MC_Samples && cd MC_Samples
rucio get user.dbaronmo.601230.PhPy8EG.DAOD_PHYS.e8514_s4162_r15540_p6697.FTAGCalib_EMuJets_B_02102025_5252165_output --ndownloader=5
```
Now just wait until the download is completed!


