# Magebit-PageListWidget
This is a Custome Module for Magento 2. 
Below are the steps I took to achieve the results I have
1. First, I created a new module using Magebit as namespace and PageListWidget as the module name and created registration.php at Magento 2_Root\app\code\Magebit\PageListWidget\directory. The file name is registration.php Below is the Code;
2. Second, I created a module.xml file at \Magebit\PageListWidget\etc\.
3. Next, I created a widget.xml configuration file at Magebit\PageListWidget\etc\with the following code. Here; I have declared three parameters, they include,  One input fields with labels Title and Two select field types with Labels Display Mode and Selcted Pages . Whatever the widget is called, it will display the value of both the fields. In the <widget> tag, I have declared a block class, \Magebit\CustomWidget\Block\Widget\Samplewidget that instructs our widget to use the particular template. 
4. Now, I  created a block file named Samplewidget.php in \Magebit\CustomWidget\Block\Widget\ directory with the following code. In this step , I have assigned a template file inside the $_template variable.
5. Finally, I created a widget template file samplewidget.phtml in \Magebit\PageListWidget\view\frontend\templates\widget . Here, as you can see that I have picked up the value from fields by calling $block->getData(‘parameter’); where the parameters are widgettitle and widgetcontent.
