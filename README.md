NakaNode
========

NakaNode simplifies setting up a Tor-enabled Bitcoin node on Windows. It's a user-friendly batch script installer that installs gpg4win, Tor, Bitcoin, and lets you choose between popular privacy-focused wallets like Wasabi or Sparrow. If you already have a preferred wallet, you can easily configure it to work with NakaNode's Tor-enabled Bitcoin node.


Features
--------

- Simplified Installation: NakaNode streamlines the installation process, allowing you to set up a Tor-enabled Bitcoin node with ease. The batch script takes care of installing gpg4win, Tor, and Bitcoin for you, eliminating the need for manual setup steps.

- Wallet Options: Choose the wallet software that best suits your needs. NakaNode gives you the option to install Wasabi or Sparrow, two popular wallet solutions known for their security and privacy features. Alternatively, you can opt to use the wallet software of your choice.

- IBD Progress Monitoring: NakaNode keeps you informed about the progress of the initial block download process. It provides regular updates and prompts you when the download and sync process is completed.

- Checksum Verification and Gpg Signatures: NakaNode prioritizes security by automatically checking the SHA256 checksums of downloaded packages and verifying their Gpg signatures using Gpg4win. This ensures the authenticity and integrity of the installed software, reducing the risk of tampering or malicious modifications.

- Exclusive Tor Network Connection: NakaNode ensures that your Bitcoin node only connects to the Bitcoin network through Tor. This exclusive connection over Tor enhances your privacy and anonymity, making it more difficult for third parties to track your activities on the Bitcoin network.

- Enhanced User Experience: NakaNode makes setting up a Tor dedicated node on Windows easier and hassle-free. With the power of batch scripting, the process is simplified, providing a seamless experience for users. Manual installations can be complex, but NakaNode's script takes care of it for you.


Installation
------------

To get started with NakaNode, follow these steps:

1. Download the latest release of NakaNode from the GitHub repository.

2. Extract the contents of the downloaded ZIP file to a location of your choice.

3. Open the extracted NakaNode folder.

4. Double click on the NakaNode-installer.exe file to launch the NakaNode installer.

5. Sit back and relax! NakaNode will handle the installation process for you, ensuring that gpg4win, Tor, and Bitcoin are installed correctly.

6. When prompted, select the wallet option that best suits your needs.
- Set up your chosen wallet according to its specific instructions.

7. Enjoy the privacy and security provided by NakaNode's Tor-enabled node package.
- Double click NakaNode.exe to start Tor and bitcoind.



Requirements
------------

NakaNode has the following requirements:

    Windows operating system (tested on Windows 10)
    - bitsadmin
    - curl
    - powershell
    Internet connection
    Sufficient storage space for the Bitcoin blockchain (1TB recommended, minimum 8-10GB with pruning enabled)



Usage
=====

Once NakaNode is installed, you can access your Tor-enabled Bitcoin node and the chosen wallet software. Here are some tips to get started:

- To access your Bitcoin node, navigate to the installation directory and run the NakaNode.exe executable.

- If you chose to install Wasabi or Sparrow, you can find their respective executables in their default installation directory or the Desktop shortcut that was created using their install wizards. Launch the wallet software of your choice to manage your Bitcoin funds securely.

- If you decided to use your existing wallet, configure it to connect to your Tor-enabled node. Ensure that the necessary network settings are adjusted to utilize the Tor network for enhanced privacy.



Creating a Shortcut for NakaNode.exe
------------------------------------

To create a shortcut for NakaNode.exe with a custom icon, follow these steps:

1. Open Windows Explorer and navigate to the location where you want to create the shortcut.

2. Right-click in the folder and select "New" and then "Shortcut". This will open the "Create Shortcut" wizard.

3. In the "Create Shortcut" wizard, click the "Browse" button and navigate to the folder where NakaNode.exe is located.

4. Once you are in the folder containing NakaNode.exe, select the file and click the "OK" button.

5. In the "Create Shortcut" wizard, you will see the location of the file in the "Target" field. By default, it should be something like "C:\Path\To\NakaNode.exe".

6. Click the "Next" button, enter a name for the shortcut (e.g., NakaNode), and click the "Finish" button to create the shortcut.

7. Right-click on the newly created shortcut and select "Properties". This will open the properties window for the shortcut.

8. In the properties window, go to the "Shortcut" tab.

9. Click the "Change Icon" button. This will open the "Change Icon" window.

10. Click the "Browse" button in the "Change Icon" window and navigate to the "icons" folder located in the NakaNode\applications directory.

11. In the "icons" folder, select the desired icon file (e.g., icon.ico) and click the "OK" button.

12. Back in the "Change Icon" window, you will see the selected icon. Click the "OK" button to apply the icon to the shortcut.

13. Click the "Apply" button and then the "OK" button in the shortcut's properties window to save the changes.

14. The shortcut for NakaNode.exe with the custom icon will be created in the folder you selected in step 1. You can now double-click the shortcut to launch NakaNode with the chosen icon.

Note: If you move the NakaNode.exe file to a different location, make sure to update the shortcut's target path and icon. Right-click on the shortcut, select "Properties," and modify the "Target" field to point to the new location of NakaNode.exe. Follow steps 7-13 to change the icon again if necessary.

By following these steps, you can easily create a shortcut for NakaNode.exe with a custom icon and conveniently launch the application from any desired location.



Privacy Considerations
======================

The Bitcoin configuration file for your node has been set to only allow network connections over Tor. This configuration is crucial for maintaining your privacy and anonymity in the Bitcoin network.

It is important to note that to fully benefit from the privacy features provided by your Tor-enabled Bitcoin node, you must ensure that any wallet software used to interact with the node is also configured to broadcast transactions using your Tor-enabled Bitcoin node or exclusively over Tor.

Why is this important?
By restricting network connections to Tor, your Bitcoin node routes all communication through the Tor network, which helps protect your IP address and hides your physical location. However, if your wallet software is not set up to use Tor, it may unknowingly broadcast transactions over the clearnet, revealing your IP address and compromising your privacy.

How to ensure your wallet software uses Tor:
1. Configure your wallet software: Review the settings of your wallet software and ensure that it is configured to communicate with your Bitcoin node exclusively over Tor. This setting is typically found in the network or connection preferences.

2. Test your setup: Before using your wallet software with your Tor-enabled Bitcoin node, perform a test transaction to confirm that the transaction is being broadcasted over Tor. You can use a blockchain explorer to check if your transaction appears as being sent from a Tor exit node.

3. Regularly verify settings: Periodically check the configuration of your wallet software to ensure that it continues to use Tor for all network communication. Software updates or changes in settings might reset the preferences, potentially exposing your transactions to the clearnet.

By following these steps, you can enhance your privacy and maintain the anonymity provided by the Tor network. Remember, privacy is a critical aspect of Bitcoin, and taking the necessary precautions ensures that your transactions remain confidential and untraceable.

Please take the time to review your wallet software's settings and ensure that it is configured to use Tor exclusively. If you have any questions or need further assistance, do not hesitate to seek support from your wallet software's documentation or community forums.

Protect your privacy, protect your Bitcoin!

Wallet Info
===========
Wasabi
------
Wasabi Wallet is designed to provide enhanced privacy and fungibility for Bitcoin transactions by default. When using Wasabi Wallet with your own Bitcoin node, the wallet establishes a direct connection to your node for block data retrieval. Here's a step-by-step explanation of how Wasabi works with your own node:
- Wasabi Wallet connects to your locally running Bitcoin node, which acts as a backend for the wallet.
- When you initiate a transaction or perform any blockchain-related operations in Wasabi Wallet, it sends requests to your Bitcoin node.
- The Bitcoin node processes these requests and retrieves the required block data from its local copy of the blockchain.
- The retrieved block data is then sent back to Wasabi Wallet, allowing it to perform transaction validation, coin selection, and other wallet operations locally.
- Finally, Wasabi Wallet broadcasts the signed transactions to the Bitcoin network using its own implementation of Tor.
Wasabi Wallet uses its own built-in Mega-CoinJoin implementation to improve transaction privacy. It combines your transactions with many other Wasabi users in a coordinated manner, making it harder to trace the origin and destination of individual coins.

- Visit https://docs.wasabiwallet.io/ for more information on Wasabi wallet.

Sparrow
-------
Sparrow wallet by default will connect to your bitcoin node using localhost 127.0.0.1. However, in order for sparrow to use Tor you will need to specify the use of a Tor proxy (port 9050 by default) To do this:
- Open Sparrow wallet and navigate to the preferences tab (Ctrl + P).
- Select Server.
- Switch on "Use Proxy" and ensure the 'Proxy url:' is set to 127.0.0.1 (localhost) 9050
- Click Test Connection. Sparrow will attempt to connect to Bitcoin Core.
Sparrow won’t use the proxy to connect to Bitcoin Core unless you specify a .onion address in the URL. But, it will use the proxy for all other external addresses, such as fetching exchange rates or using Whirlpool. Sparrow sends transactions to your local Bitcoin node to be broadcasted to the network.

Whirlpool is an advanced privacy feature offered by Sparrow Wallet. It allows you to Coinjoin with other users.
When you participate in a Whirlpool mix, Sparrow Wallet utilizes the Tor-enabled Bitcoin node to communicate with other participants anonymously, enhancing the privacy of your transactions.
By utilizing the Tor network and the Whirlpool feature, Sparrow Wallet provides an additional layer of privacy and fungibility to your Bitcoin transactions.

- Visit https://www.sparrowwallet.com/docs/mixing-whirlpool.html for more information of how to use Whirlpool in Sparrow wallet.

Contributing
============

Contributions to NakaNode are welcome! If you encounter any issues, have suggestions, or want to contribute improvements, please feel free to create an issue or submit a pull request on the GitHub repository.
Disclaimer

NakaNode is provided as-is, without any warranties or guarantees. Use the software at your own risk. The developers and contributors to NakaNode are not responsible for any loss or damages incurred during the installation or usage of the software.
License

NakaNode is open-source software released under the MIT License. Feel free to use, modify, and distribute the software in accordance with the terms of the license.



## Disclaimer

NakaNode is provided as-is, without any warranties or guarantees. Use the software at your own risk. The developers and contributors to NakaNode are not responsible for any loss or damages incurred during the installation or usage of the software.

## License

NakaNode is open-source software released under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use, modify, and distribute the software in accordance with the terms of the license.
