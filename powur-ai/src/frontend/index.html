<!DOCTYPE html>
<html lang="en">

<head>
    <title>Powur AI Demo</title>
    <meta name="description" content="Powur-AI-Demo">


<meta name="viewport" content="width=device-width; maximum-scale=1.0; initial-scale=1.0; user-scalable=0;">


    <style> :not(:defined) {visibility: hidden; } </style>
    <link rel="shortcut icon" href="favicon.gif">
    <!-- Web Components by Shoelace: https://shoelace.style -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@shoelace-style/shoelace@2.0.0/dist/themes/light.css" />
    <script type="module" src="https://cdn.jsdelivr.net/npm/@shoelace-style/shoelace@2.0.0/dist/shoelace.js"></script>
    <link rel="stylesheet" href="styles.css">
    <script src="scripts.js" defer></script>
</head>

<body>

<div class="float-container" style="float: left">

<div style="align: left">

<style>img.thatimage
{
    max-width: 60%;
    min-width: 80px;
    height: auto;
}</style>


<img class="thatimage" style="scaledown" alt="Powur.com" src="favicon.gif">
<h4>Powur AI Demo</h4>

</div>  
</div><br>
    <sl-card style="align:right">
        <div slot="header">Input</div>
        <sl-select hoist id="location" label="Location"></sl-select>
        <sl-select hoist id="processor" label="Processor"></sl-select>
        <span id="document"><span>Document</span>
            <sl-button-group label="Document">
                <sl-button id="files" variant="success">
                    <sl-icon slot="prefix" name="file-earmark-arrow-up"></sl-icon>File(s)
                </sl-button>
                <sl-dropdown>
                    <sl-button slot="trigger" caret>
                        <sl-icon slot="prefix" name="file-earmark-arrow-down">
                        </sl-icon>Sample
                    </sl-button>
                    <sl-menu id="samples"></sl-menu>
                </sl-dropdown>
            </sl-button-group>
        </span>
    </sl-card> 
    <sl-card id="output-card">
        <div slot="header">Output

            
            <div class="float-container" style="float: left; margin-right: 5px; text-align: left;">
                <div class="details-group-example">
                <sl-details variant="default" size="small" style="width: 100%; margin-top: 0.25rem;"
                summary="DETAILS. Click to expand">
                <h3>## !*!* Select 'Entities' from Overlay menu below to display an animated output *!*! ##</h3>
                <h4>- Wait up to 10 seconds after upload for response to process.</h4>
                <h5>- Additional options available by clicking the 3 dots to the right.</h5>
                <h5>- If you don't have a bill on hand, click "Sample" dropdown to select a pre-uploaded example.</h5>
                <h5>- Some samples were intentionally uploaded blurry, to showcase the flexibility of the processor.</h5>
                <h5>- Spanish was never trained into the machine learning model at all, however one of the samples is printed in spanish, also to demonstrate flexibility.</h5>
                </sl-details>
                <sl-details variant="default" size="small" style="width: 100%; margin-top: 0.25rem;"
                summary="Disclaimer / Explanation of Pitfalls">
                <h5>- Due to the thin paper, and the reverse side text bleeding through, The SCE bill for Van wasn't able to identify the name field (as a special entity). When the full UB is uploaded, the processor correctly identifies the customer name in many different pages,
                    and confirms they all match to confirm the accuracy of its findings. If the full bill had been uploaded, the processor would have located and marked the customer name on this page as well. 
                    This would be completely eliminated with additional training of the processor model.</h5>
                <h5>Understand that the "entities" fields are specialized fields, which have been custom trained to identify and seperate a few key data fields and extract them out into their own datapoints to allow for automated entry into a database.
                    The fact that the customer name is not labeled, is completely intentional. The confidence of the field value is under the specified threshold, 
                    which prevents incorrect data from entering the final dataset. The customers name was in fact correctly read out, which you can verify on the "text" tab to the right. 
                    The processor just wasn't confident enough to label the field as a specialized "entity"
                    This document would then be forwarded on to a representative who would perform a manual review, before sending it back to the processor, to further train the machine learning model for better future results.
                </h5>
                    <h5>Also, the meter # wasn't identified on the SDGE bill. This would also be a non-issue after further training. The processor was only trained with a small # of samples for SDGE. with 10 more, that issue would be eliminated.</h5>
                    <h3>The samples are single pages, I encourage you to upload test documents which include all the pages, for a better representation.</h3>
                    <h4>In both of these examples, the processor still correctly read out this information into searchable raw text form, which you can verify on the "text" tab to the right. Further showing that additional up-training would solve those issues</h4>
                </sl-details>
                <script>
                    const container = document.querySelector('.details-group-example');
                    // Close all other details when one is shown
                    container.addEventListener('sl-show', event => {
                        [...container.querySelectorAll('sl-details')].map(details => (details.open = event.target === details));
                    });
                </script>
                </div>
                </div>
            <sl-dropdown>
                <sl-icon slot="trigger" name="three-dots-vertical" style="font-size: 2.5rem;"></sl-icon>
                <sl-menu id="options">
                    <sl-menu-label>Source code</sl-menu-label>
                    <sl-menu-item id="source-code">View on GitHub
                        <sl-icon slot="prefix" name="box-arrow-up-right">
                        </sl-icon></sl-menu-item>
                    <sl-divider></sl-divider>
                    <sl-menu-label>Download</sl-menu-label>
                    <sl-menu-item id="download-docai-json">Json Format
                        <sl-icon slot="prefix" name="file-earmark-arrow-down"></sl-icon>
                    </sl-menu-item>
                    <sl-menu-item id="download-output-image">Output image
                        <sl-icon slot="prefix" name="file-earmark-arrow-down"></sl-icon>
                    </sl-menu-item>
                    <sl-divider></sl-divider>
                    <sl-menu-label>Output options</sl-menu-label>
                    <sl-menu-item value="animated" type="checkbox"checked>Animated
                        <sl-icon slot="prefix" name="film"></sl-icon>
                    </sl-menu-item>
                    <sl-menu-item value="cropped" type="checkbox">Cropped to text
                        <sl-icon slot="prefix" name="crop"></sl-icon>
                    </sl-menu-item>
                    <sl-menu-item value="confidence" type="checkbox" checked>Confidence
                        <sl-icon slot="prefix" name="percent"></sl-icon>
                    </sl-menu-item>
                    <sl-menu-item value="normalized" type="checkbox">Normalized values
                        <sl-icon slot="prefix" name="rulers"></sl-icon>
                    </sl-menu-item>
                    <sl-divider></sl-divider>
                    <sl-menu-label>Output format</sl-menu-label>
                </sl-menu>
            </sl-dropdown>
        </div>
        <sl-tab-group placement="end">
            <sl-tab slot="nav" panel="page">Page</sl-tab>
            <sl-tab slot="nav" panel="text">Text</sl-tab>
            <sl-tab slot="nav" panel="document">Doc.</sl-tab>
            <sl-tab-panel name="page">
                <sl-select hoist id="page" label="Page"></sl-select>
                <sl-select hoist id="overlay" label="Overlay" value="no-info">
                    <sl-option value="no-info">-None-</sl-option>
                    <sl-option value="blocks">Blocks (0)</sl-option>
                    <sl-option value="paragraphs">Paragraphs (0)</sl-option>
                    <sl-option value="lines">Lines (0)</sl-option>
                    <sl-option value="tokens">Tokens (0)</sl-option>
                    <sl-option value="tables">Tables (0)</sl-option>
                    <sl-option value="barcodes">Barcodes (0)</sl-option>
                    <sl-option value="fields">Form fields (0)</sl-option>
                    <sl-option value="entities">Entities (0)</sl-option>
                </sl-select>
                <img id="output-image" alt="output image">
            </sl-tab-panel>
            
                    <sl-tab-panel name="text">
                        <sl-textarea id="document-text" 
                        placeholder="document.text" rows="6" 
                        readonly></sl-textarea></sl-tab-panel>
                    <sl-tab-panel name="document">
                        <sl-tree id="document-tree"></sl-tree>
                    </sl-tab-panel>
                    
                </sl-tab-group>
                </sl-card>
            <sl-dialog id="dialog" label="Focus on the document (at any angle)">
                <video id="video" playsinline></video>
                <sl-button id="snapshot" slot="footer" size="large">
                    <sl-icon slot="prefix" name="camera"></sl-icon>Snapshot
                </sl-button>
            </sl-dialog>
    </body>
</html>
