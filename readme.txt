// *************************************************************************
// * Modding Unlimited Air Mail 5 module for phpVMS                        *
// * Copyright (c) Hurkulez (moddingunlimited.net) All Rights Reserved     *
// * Release Date: 11 April 2016                                           *
// * Version 1.00                                                          *
// * Email: hurkulez@gmail.com                                             *
// * Website: http://www.moddingunlimited.net                              *
// *************************************************************************
// * This software is furnished under a license and may be used and copied *
// * in  accordance  with  the  terms  of such  license and with the       *
// * inclusion of the above copyright notice.                              *
// *************************************************************************

This system is not compatible with any earlier versions of AirMail

New Features:

-Delete All function in inbox and all message folders
-Individual pilot setting to have email sent to pilot when new message is received
-Threaded messages

Install Using Simpilotgroup Plugin Manager

-Download the package
-Upload the package to your site using the plugin manager
-Use the auto-install from the plugin manager

Install Manually:

-Download the package.
-Unzip the package and place the files as structured in your root phpVMS install.
-Use the airmail.sql file to create the tables needed in your sql database using phpmyadmin or similar.

Options:

To Use the "You Have Mail" function place the following code where you would like the notice to appear, it will only appear if the pilot is logged in.

<?php MainController::Run('Mail', 'checkmail'); ?>

-Create a link on your site for your pilots to access their AIRMail

<a href="<?php echo url('/Mail'); ?>">AIRMail</a>