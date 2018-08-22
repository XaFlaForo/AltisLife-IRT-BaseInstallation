<p>
<h3 align="center">Altis Life: IRT Base Installation</h3>
</p>
<h3> Synopsis:</h3>
To install any script with (IRT) in its name you must install this dependency first

<h3> Installation Guide</h3>

<b> Step 1: DOWNLOAD THE IRT FOLDER AND PUT IT IN THE ROOT OF YOUR MISSION </b>
<br/> 


<b> Step 2: GO TO description.ext AND PASTE THE CODE BELOW AT TOP OF THE FILE </b>

<br/> 

#include "IRT\IRT_Config.hpp"

<br/> 

<b> Step 3: GO TO description.ext AND PASTE THE CODE BELOW IN CfgFunctions </b>

<br/> 

#include "IRT\IRT_Functions.hpp"

<br/> 


<br/> 
<b> Step 4: GO TO CfgRemoteExec.hpp AND PASTE THE CODE BELOW jip = 0; </b>

<br/> 
<br/> 
#include "IRT\IRT_RemoteExec.hpp"

<br/> 

## Copyright and License

Copyright (c) 2018 Ethan (XaLaForo), IRT Studios

### All code is licensed under the MIT license.
