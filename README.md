# tycho-eclipse-learning
pratice of https://www.vogella.com/tutorials/EclipseTycho/article.html#pre-requirements-for-this-tutorial

#F&Q
* tycho generated config.ini does not start runtime 
http://software.2206966.n2.nabble.com/tycho-generated-config-ini-does-not-start-runtime-td6077893.html
Please check from .product->Contents Tab, if any issue with red cross, linux macos native will be included but can not find base on your eclipse downloaded, you can remove them manually, but you can package .win32, linux, macos products togethers though you are using eclispe-win32.

* [ERROR] Cannot resolve dependencies of product com.vogella.tycho.rcp.product:
* [ERROR]   eclipse-plugin artifact with ID "org.eclipse.core.filesystem" and version matching "0.0.0" was not found in the target platform
* [ERROR]   eclipse-plugin artifact with ID "org.eclipse.core.resources" and version matching "0.0.0" was not found in the target platform
* [ERROR]   eclipse-plugin artifact with ID "org.eclipse.core.filesystem.win32.x86_64" and version matching "0.0.0" was not found in the target platform
* [ERROR] Failed to execute goal org.eclipse.tycho:tycho-p2-publisher-plugin:1.5.1:publish-products (default-publish-products) on project com.vogella.tycho.product: Execution 
* default-publish-products of goal org.eclipse.tycho:tycho-p2-publisher-plugin:1.5.1:publish-products failed: Cannot resolve dependencies of product com.vogella.tycho.rcp.product. See log for 
* details. -> [Help 1]

in product configuration, used based on feature.