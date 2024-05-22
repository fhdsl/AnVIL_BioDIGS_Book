




# Using Galaxy on AnVIL

In the next few steps, you will walk through how to get set up to use Galaxy on the AnVIL platform. AnVIL is centered around different “Workspaces”. Each Workspace functions almost like a mini code laboratory - it is a place where data can be examined, stored, and analyzed. The first thing we want to do is to copy or “clone” a Workspace to create a space for you to experiment.

Use a web browser to go to the AnVIL website. In the browser type:

```
anvil.terra.bio
```

:::{.notice}
**Tip**
At this point, it might make things easier to open up a new window in your browser and split your screen. That way, you can follow along with this guide on one side and execute the steps on the other.
:::

Your instructor will give you information on which workspace you should clone. After logging in, click “View Workspaces”. Select the “Public” tab.  In the top search bar type the activity workspace. 

Clone the workspace by clicking the teardrop button (![teardrop button](resources/images/teardrop.png){#id .class width=25 height=20px}). And selecting “Clone”.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_ged15532ded_0_625.png" title="Screenshot showing the teardrop button. The button has been clicked revealing the &quot;clone&quot; option. The Clone option and the teardrop button are highlighted." alt="Screenshot showing the teardrop button. The button has been clicked revealing the &quot;clone&quot; option. The Clone option and the teardrop button are highlighted." width="480" />

In the first box, give your Workspace clone a name by adding an underscore (“_”) and your name. For example, “SARS-CoV-2-Genome_Ava_Hoffman”. Next, select the Billing project provided by your instructor. Leave the bottom two boxes as-is and click “CLONE WORKSPACE”.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_ged15532ded_0_648.png" title="Screenshot showing the &quot;clone a workspace&quot; popout. The Workspace name, Billing Project, and Clone Workspace button have been filled in and highlighted." alt="Screenshot showing the &quot;clone a workspace&quot; popout. The Workspace name, Billing Project, and Clone Workspace button have been filled in and highlighted." width="480" />

## Video overview on using Galaxy


Here is a video tutorial that describes the basics of using Galaxy on AnVIL.

<iframe src="https://drive.google.com/file/d/16QEY8x-gBsUkKEeO3w_H-I4SLIBPloXd/preview" width="640" height="360" allow="autoplay"></iframe>

### Objectives

- Start compute for your Galaxy on AnVIL
- Run tool to quality control sequencing reads
- Stop compute to minimize expenses

### Slides

The slides for this tutorial are are located [here](https://docs.google.com/presentation/d/1yYCg4cPVBMMDghT17B4XzROieqyMH99Ex9nMm_Scm9Q).


## Starting Galaxy {#starting-galaxy}

Galaxy is a free, relatively easy to use bioinformatics implementation package. It changes command line programs into GUI based programs and is a great tool for performing bioinformatics analysis without having to update software or worry too much about coding. In order to use Galaxy, we need to create a cloud environment. This is like quickly renting a few computers from Google as the engine to power our Galaxy analysis. 

:::{.warning}
Currently, you will need to use Chrome or Safari as your browser for Galaxy cloud environments to work.
:::

In your new Workspace, click on the “ANALYSES” tab. Next, click on “START”. You should see a popup window on the right side of the screen. Click on the Galaxy logo to proceed.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_ged15532ded_0_788.png" title="Screenshot of the Workspace Notebooks tab. The notebook tab name and the plus button that starts a cloud environment for Galaxy have been highlighted," alt="Screenshot of the Workspace Notebooks tab. The notebook tab name and the plus button that starts a cloud environment for Galaxy have been highlighted," width="480" />

Click on “NEXT” and “CREATE” to keep all settings as-is.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_ged15532ded_0_798.png" title="The CREATE button among cloud environments has been highlighted." alt="The CREATE button among cloud environments has been highlighted." width="480" />

Click on the Galaxy icon. 

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_g2283b458fae_100_31.png" title="The Galaxy icon appears if the environment has been successfully launched." alt="The Galaxy icon appears if the environment has been successfully launched." width="480" />

You will see that the environment is still being set up.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_g2283b458fae_100_38.png" title="The status of the cloud computing environment shows that it is still being set up." alt="The status of the cloud computing environment shows that it is still being set up." width="480" />

This will take 8-10 minutes. When it is done, click “Open”. You might need to refresh the page.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_g2283b458fae_100_46.png" title="The Provisioning status text has changed to &quot;Launch Galaxy&quot; indicating the cloud environment is ready to use." alt="The Provisioning status text has changed to &quot;Launch Galaxy&quot; indicating the cloud environment is ready to use." width="480" />

:::{.notice}
Remember that you can refresh your browser or navigate away at any time. This is because the connection to the environment is in the cloud, not on your personal computer.
:::

You can also follow along with the first ~2 minutes of [this video](https://jhudatascience.org/AnVIL_Book_Getting_Started/starting-galaxy.html) to start Galaxy on AnVIL.

## Navigating Galaxy

Notice the three main sections.

**Tools** - These are all of the bioinformatics tool packages available for you to use.

**The Main Dashboard** - This contains flash messages and posts when you first open Galaxy, but when we are using data this is the main interface area.

**History** - When you start a project you will be able to see all of the documents in the project in the history. Now be aware, this can become very busy. Also the naming that Galaxy uses is not very intuitive, so you must make sure that you label your files with something that makes sense to you.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_ged15532ded_0_816.png" title="Screenshot of the Galaxy landing page. The Tools and History headings have been highlighted." alt="Screenshot of the Galaxy landing page. The Tools and History headings have been highlighted." width="480" />

On the welcome page, there are links to tutorials. You may try these out on your own. If you want to try a new analysis this is a good place to start.

## Deleting Galaxy


Once you are done with your activity, you’ll need to shut down your Galaxy cloud environment. This frees up the cloud resources for others and minimizes computing cost. The following steps will delete your work, so make sure you are completely finished at this point. Otherwise, you will have to repeat your work from the previous steps.

Return to AnVIL, and find the Galaxy logo that shows your cloud environment is running. Click on this logo:

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_gf243efded1_0_134.png" title="Screenshot of the Workspace menu. The currently running Galaxy cloud environment logo on the top right of the page is highlighted." alt="Screenshot of the Workspace menu. The currently running Galaxy cloud environment logo on the top right of the page is highlighted." width="480" />

Next, click on “DELETE ENVIRONMENT OPTIONS”:

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_gf243efded1_0_140.png" title="Screenshot of the cloud environment pop out menu. The “DELETE ENVIRONMENT OPTIONS” link is highlighted." alt="Screenshot of the cloud environment pop out menu. The “DELETE ENVIRONMENT OPTIONS” link is highlighted." width="480" />

Finally, select “Delete everything, including persistent disk”. Make sure you are done with the activity and then click “DELETE”.

<img src="resources/images/08-student_using_galaxy_files/figure-html//182AOzMaiyrreinnsRX2VhH7YsVgvAp4xtIB_7Mzmk6I_gf243efded1_0_146.png" title="Screenshot of the cloud environment pop out menu. The “Delete everything, including persistent disk” radio button has been checked and is highlighted. The “DELETE” button is highlighted." alt="Screenshot of the cloud environment pop out menu. The “Delete everything, including persistent disk” radio button has been checked and is highlighted. The “DELETE” button is highlighted." width="480" />

