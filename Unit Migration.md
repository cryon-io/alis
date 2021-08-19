# Migration from unit
1. [Get Alis](https://github.com/cryon-io/alis/releases/tag/0.0.4), install it, run it and create an account
*NOTE: If you do not want to use alis app use it for migration and delete afterwards.*
2. Go to Machines in the left menu and add your VPS by clicking Add Machine button and set it up with your credentials
3. Click terminal >_ button to verify terminal connectivity
4. Open terminal and stop all unit nodes you want to migrate and note down their IPs
    - `unit stop [app id]` to stop a given app or `unit stop` to stop every unit app
    - All details about nodes you get get by running `cat /etc/unit/unit.json` in terminal
5. Return to Machines and open the machine on which you want to add nodes
6. In left top menu under machine id click 3 dots and select `Install alis-cli`
7. Click `Add New Application` button under Applications section
8. Set new application id and select correct application template and edit it to reflect your requirements
    - set node type and outbound address to correct values (*No need to specify outbound address if you run only one ETHO node per VPS*)
9. Save by clicking on the bottom-right button
10. In left top menu between your machine id and your machine IP adress, click 3 dots and select `Push Configuration`
11. Mouseover the 3 little stars next to your application and select `Setup` and wait until complete
12. After successful setup mouseover the 3 little stars again and select `Start` and wait until complete
14. Wait for sync. You can refresh app status by click the reload button next to the 3 little stars or in header of application section