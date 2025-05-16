<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Note Template Generator</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f7fa;
        }
        
        h1 {
            color: #2c3e50;
            text-align: center;
            margin-bottom: 30px;
        }
        
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }
        
        .form-section, .preview-section {
            background-color: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .preview-section {
            position: relative;
        }
        
        h2 {
            color: #3498db;
            margin-top: 0;
            border-bottom: 2px solid #f0f0f0;
            padding-bottom: 10px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .conditional-field {
            padding: 15px;
            border-left: 3px solid #3498db;
            background-color: #f1f9ff;
            display: none;
        }
        
        .add-more-link {
            color: #3498db;
            cursor: pointer;
            font-weight: 600;
            display: inline-block;
            margin-top: 10px;
            margin-bottom: 20px;
            text-decoration: underline;
        }
        
        .delete-group-btn {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 5px 10px;
            font-size: 14px;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
            margin-bottom: 20px;
        }
        
        .additional-part-group {
            border-left: 3px solid #3498db;
            padding-left: 15px;
            margin-bottom: 30px;
            background-color: #f8f9fa;
            padding: 15px;
            border-radius: 4px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #555;
        }
        
        input[type="text"], textarea, select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: inherit;
            font-size: 15px;
            box-sizing: border-box;
        }
        
        textarea {
            min-height: 100px;
            resize: vertical;
        }
        
        .btn {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 12px 20px;
            font-size: 16px;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        .btn-copy {
            background-color: #27ae60;
            margin-left: 10px;
        }
        
        .btn-copy:hover {
            background-color: #219653;
        }
        
        .btn-reset {
            background-color: #e74c3c;
        }
        
        .btn-reset:hover {
            background-color: #c0392b;
        }
        
        .button-group {
            display: flex;
            margin-top: 20px;
            gap: 10px;
        }
        
        #preview {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: 4px;
            border: 1px solid #e0e0e0;
            min-height: 300px;
            white-space: pre-wrap;
            font-family: 'Courier New', monospace;
            font-size: 14px;
            margin-top: 15px;
            overflow-y: auto;
            line-height: 1.5;
        }
        
        .copy-message {
            position: absolute;
            top: 25px;
            right: 25px;
            background-color: #27ae60;
            color: white;
            padding: 8px 12px;
            border-radius: 4px;
            font-size: 14px;
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .copy-message.show {
            opacity: 1;
        }
        
        .template-controls {
            margin-bottom: 30px;
        }
        
        select {
            padding: 10px;
            border-radius: 4px;
            border: 1px solid #ddd;
            font-size: 15px;
            margin-right: 10px;
        }

        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <h1>Note Template Generator</h1>
    
    <div class="container">
        <div class="form-section">
            <h2>Template Input</h2>
            
            <div class="template-controls">
                <label for="template-select">Choose a template:</label>
                <select id="template-select">
                    <option value="breakfix">Break/Fix Task Notes</option>
                    <option value="networking">Networking Task Notes</option>
                    <option value="meeting">Meeting Note</option>
                    <option value="project">Project Update</option>
                    <option value="workwindow">Work Window Request Email</option>
                    <option value="custom">Custom Template</option>
                </select>
            </div>
            
            <form id="template-form">
                <!-- Fields will be dynamically generated here -->
            </form>
        </div>
        
        <div class="preview-section">
            <h2>Note Preview</h2>
            <div id="preview">Your compiled note will appear here...</div>
            <div class="button-group">
                <button type="button" class="btn" id="complete-btn">Complete Note</button>
                <button type="button" class="btn btn-copy" id="copy-btn">Copy to Clipboard</button>
                <button type="button" class="btn btn-reset" id="reset-btn">Reset</button>
            </div>
            <div class="copy-message" id="copy-message">Note copied to clipboard!</div>
        </div>
    </div>

    <script>
        // Template definitions
        const templates = {
            breakfix: {
                title: "Break/Fix Task Notes",
                fields: [
                    { name: "taskId", label: "Task ID", type: "text" },
                    { name: "assetTagConfirmed", label: "Was the asset tag visually confirmed?", type: "select", options: ["Yes", "No"] },
                    { name: "taskReviewed", label: "Did you review the task?", type: "select", options: ["Yes", "No"] },
                    { name: "notesReviewed", label: "Did you review the notes?", type: "select", options: ["Yes", "No"] },
                    { name: "uponArrival", label: "Upon Arrival:", type: "textarea" },
                    { name: "partReplaced", label: "Part(s) Replaced", type: "text" },
                    { name: "oldSerialNumber", label: "Old Serial Number", type: "text" },
                    { name: "newSerialNumber", label: "New Serial Number", type: "text" },
                    { name: "licensePlate", label: "License Plate", type: "text" },
                    { name: "actionsTaken", label: "Actions Taken", type: "textarea" },
                    { name: "wasEscalated", label: "Was this ticket escalated?", type: "select", options: ["Yes", "No"], hasConditionalFields: true },
                    { name: "escalatedTo", label: "Who will this be escalated to?", type: "text", conditionalOn: { field: "wasEscalated", value: "Yes" } },
                    { name: "seniorTechAlias", label: "Senior Technician Alias who approved escalation", type: "text", conditionalOn: { field: "wasEscalated", value: "Yes" } }
                ],
                format: (data) => {
                    let escalationInfo = "";
                    if (data.wasEscalated === "Yes") {
                        escalationInfo = `
ESCALATION DETAILS:
- Escalated To: ${data.escalatedTo || "[Not specified]"}
- Senior Tech Approval: ${data.seniorTechAlias || "[Not specified]"}`;
                    }
                    
                    return `TASK ID: ${data.taskId || "[No ID]"}
ASSET TAG CONFIRMED: ${data.assetTagConfirmed || "N/A"}
TASK REVIEWED: ${data.taskReviewed || "N/A"}
NOTES REVIEWED: ${data.notesReviewed || "N/A"}

UPON ARRIVAL:
${data.uponArrival || "[No arrival notes recorded]"}

PART(S) REPLACED: ${data.partReplaced || "N/A"}
OLD SERIAL NUMBER: ${data.oldSerialNumber || "N/A"}
NEW SERIAL NUMBER: ${data.newSerialNumber || "N/A"}
LICENSE PLATE: ${data.licensePlate || "N/A"}

ACTIONS TAKEN:
${data.actionsTaken || "[No actions recorded]"}

TICKET ESCALATED: ${data.wasEscalated || "No"}${escalationInfo}`;
                }
            },
            networking: {
                title: "Networking Task Notes",
                fields: [
                    { name: "taskId", label: "Task ID", type: "text" },
                    { name: "assetTagConfirmed", label: "Was the asset tag visually confirmed?", type: "select", options: ["Yes", "No"] },
                    { name: "taskReviewed", label: "Did you review the task?", type: "select", options: ["Yes", "No"] },
                    { name: "notesReviewed", label: "Did you review the notes?", type: "select", options: ["Yes", "No"] },
                    { name: "uponArrival", label: "Upon Arrival:", type: "textarea" },
                    { name: "sourceDevice", label: "Source Device:Port", type: "text" },
                    { name: "endDevice", label: "End Device:Port", type: "text" },
                    { name: "partReplaced", label: "Part(s) Replaced", type: "text" },
                    { name: "oldSerialNumber", label: "Old Serial Number", type: "text" },
                    { name: "newSerialNumber", label: "New Serial Number", type: "text" },
                    { name: "licensePlate", label: "License Plate", type: "text" },
                    { name: "actionsTaken", label: "Actions Taken", type: "textarea" },
                    { name: "wasEscalated", label: "Was this ticket escalated?", type: "select", options: ["Yes", "No"], hasConditionalFields: true },
                    { name: "escalatedTo", label: "Who will this be escalated to?", type: "text", conditionalOn: { field: "wasEscalated", value: "Yes" } },
                    { name: "seniorTechAlias", label: "Senior Technician Alias who approved escalation", type: "text", conditionalOn: { field: "wasEscalated", value: "Yes" } }
                ],
                format: (data) => {
                    let escalationInfo = "";
                    if (data.wasEscalated === "Yes") {
                        escalationInfo = `
ESCALATION DETAILS:
- Escalated To: ${data.escalatedTo || "[Not specified]"}
- Senior Tech Approval: ${data.seniorTechAlias || "[Not specified]"}`;
                    }
                    
                    return `TASK ID: ${data.taskId || "[No ID]"}
ASSET TAG CONFIRMED: ${data.assetTagConfirmed || "N/A"}
TASK REVIEWED: ${data.taskReviewed || "N/A"}
NOTES REVIEWED: ${data.notesReviewed || "N/A"}

UPON ARRIVAL:
${data.uponArrival || "[No arrival notes recorded]"}

SOURCE DEVICE:PORT: ${data.sourceDevice || "N/A"}
END DEVICE:PORT: ${data.endDevice || "N/A"}
PART(S) REPLACED: ${data.partReplaced || "N/A"}
OLD SERIAL NUMBER: ${data.oldSerialNumber || "N/A"}
NEW SERIAL NUMBER: ${data.newSerialNumber || "N/A"}
LICENSE PLATE: ${data.licensePlate || "N/A"}

ACTIONS TAKEN:
${data.actionsTaken || "[No actions recorded]"}

TICKET ESCALATED: ${data.wasEscalated || "No"}${escalationInfo}`;
                }
            },
            meeting: {
                title: "Meeting Note",
                fields: [
                    { name: "meetingTitle", label: "Meeting Title", type: "text" },
                    { name: "date", label: "Date & Time", type: "text" },
                    { name: "attendees", label: "Attendees", type: "text" },
                    { name: "agenda", label: "Agenda", type: "textarea" },
                    { name: "decisions", label: "Key Decisions", type: "textarea" },
                    { name: "actionItems", label: "Action Items", type: "textarea" }
                ],
                format: (data) => {
                    return `MEETING: ${data.meetingTitle || "[No Title]"}
DATE: ${data.date || "N/A"}
ATTENDEES: ${data.attendees || "N/A"}

AGENDA:
${data.agenda || "[No agenda items]"}

KEY DECISIONS:
${data.decisions || "[No decisions recorded]"}

ACTION ITEMS:
${data.actionItems || "[No action items]"}`;
                }
            },
            project: {
                title: "Project Update",
                fields: [
                    { name: "projectName", label: "Project Name", type: "text" },
                    { name: "status", label: "Current Status", type: "text" },
                    { name: "accomplishments", label: "Recent Accomplishments", type: "textarea" },
                    { name: "challenges", label: "Current Challenges", type: "textarea" },
                    { name: "nextSteps", label: "Next Steps", type: "textarea" },
                    { name: "resources", label: "Required Resources", type: "textarea" }
                ],
                format: (data) => {
                    return `PROJECT UPDATE: ${data.projectName || "[No Project Name]"}
STATUS: ${data.status || "N/A"}

RECENT ACCOMPLISHMENTS:
${data.accomplishments || "[None recorded]"}

CURRENT CHALLENGES:
${data.challenges || "[None recorded]"}

NEXT STEPS:
${data.nextSteps || "[None planned]"}

REQUIRED RESOURCES:
${data.resources || "[None specified]"}`;
                }
            },
            custom: {
                title: "Custom Template",
                fields: [
                    { name: "customTitle", label: "Note Title", type: "text" },
                    { name: "customTemplate", label: "Custom Template (Use ## to denote where input values will go)", type: "textarea" },
                    { name: "customValues", label: "Values (one per line, in order of ##)", type: "textarea" }
                ],
                format: (data) => {
                    let result = `${data.customTitle || "Custom Note"}\n\n`;
                    
                    if (data.customTemplate) {
                        let template = data.customTemplate;
                        const values = data.customValues ? data.customValues.split('\n').filter(v => v.trim()) : [];
                        
                        values.forEach((value, index) => {
                            template = template.replace('##', value);
                        });
                        
                        // Replace any remaining ## with blank
                        template = template.replace(/##/g, '[empty]');
                        
                        result += template;
                    } else {
                        result += "[No custom template defined]";
                    }
                    
                    return result;
                }
            },
            workwindow: {
                title: "Work Window Request Email",
                fields: [
                    { name: "taskId", label: "Task ID", type: "text" },
                    { name: "date", label: "Date", type: "text" },
                    { name: "time", label: "Time", type: "text" }
                ],
                format: (data) => {
                    return `WORK WINDOW REQUEST - TASK ID: ${data.taskId || "[No ID]"}

Hello, 

We need to schedule a work window for task # ${data.taskId || "SlotA"}. The next available date we have for this work window is ${data.date || "SlotB"} at ${data.time || "SlotC"}. Does this work for you? 

NOTE: For every work window we will need a MINIMUM of 24 hours' notice so that SS can confirm availability. Important! Please remove traffic if necessary to facilitate a timely start for the WW event.`;
                }
            }
        };

        // Current template
        let currentTemplate = 'breakfix';
        let additionalPartsCounter = 0;
        
        // DOM elements
        const templateForm = document.getElementById('template-form');
        const previewDiv = document.getElementById('preview');
        const templateSelect = document.getElementById('template-select');
        const completeBtn = document.getElementById('complete-btn');
        const copyBtn = document.getElementById('copy-btn');
        const resetBtn = document.getElementById('reset-btn');
        const copyMessage = document.getElementById('copy-message');
        
        // Initialize with the default template
        generateFormFields();
        
        // Add change event listener to the template select
        templateSelect.addEventListener('change', changeTemplate);
        
        // Function to change template
        function changeTemplate() {
            currentTemplate = templateSelect.value;
            generateFormFields();
            updatePreview();
            if (currentTemplate === 'breakfix' || currentTemplate === 'networking') {
                ensureAddMoreButtonIsLast();
            }
        }
        
        // Function to generate form fields based on selected template
        function generateFormFields() {
            templateForm.innerHTML = '';
            additionalPartsCounter = 0;
            
            const template = templates[currentTemplate];
            
            template.fields.forEach((field, index) => {
                // Skip conditional fields initially
                if (field.conditionalOn && !shouldShowConditionalField(field)) {
                    return;
                }
                
                const formGroup = document.createElement('div');
                formGroup.className = 'form-group';
                if (field.conditionalOn) {
                    formGroup.className += ' conditional-field';
                    formGroup.setAttribute('data-depends-on', field.conditionalOn.field);
                    formGroup.setAttribute('data-depends-value', field.conditionalOn.value);
                }
                
                const label = document.createElement('label');
                label.setAttribute('for', field.name);
                label.textContent = field.label;
                
                let input;
                if (field.type === 'textarea') {
                    input = document.createElement('textarea');
                } else if (field.type === 'select' && field.options) {
                    input = document.createElement('select');
                    // Add an empty option first
                    const emptyOption = document.createElement('option');
                    emptyOption.value = '';
                    emptyOption.textContent = '-- Select --';
                    input.appendChild(emptyOption);
                    
                    // Add the rest of the options
                    field.options.forEach(optionText => {
                        const option = document.createElement('option');
                        option.value = optionText;
                        option.textContent = optionText;
                        input.appendChild(option);
                    });
                    
                    // For fields that trigger conditional fields
                    if (field.hasConditionalFields) {
                        input.addEventListener('change', handleConditionalFields);
                    }
                } else {
                    input = document.createElement('input');
                    input.type = field.type;
                }
                
                input.id = field.name;
                input.name = field.name;
                input.addEventListener('input', updatePreview);
                
                formGroup.appendChild(label);
                formGroup.appendChild(input);
                templateForm.appendChild(formGroup);
                
                // Create container for additional parts after the License Plate field
                if (field.name === 'licensePlate' && (currentTemplate === 'breakfix' || currentTemplate === 'networking')) {
                    // Add container for additional parts
                    const additionalPartsContainer = document.createElement('div');
                    additionalPartsContainer.id = 'additional-parts-container';
                    templateForm.appendChild(additionalPartsContainer);
                    
                    // Add the "Add More Parts" link initially after the main part fields
                    addAddMoreButton(templateForm);
                }
            });
        }
        
        // Function to add the "Add More Parts" button
        function addAddMoreButton(parentElement) {
            // Remove any existing add more button first
            const existingButton = document.getElementById('add-more-container');
            if (existingButton) {
                existingButton.remove();
            }
            
            // Create a new add more button
            const addMoreContainer = document.createElement('div');
            addMoreContainer.id = 'add-more-container';
            
            const addMoreLink = document.createElement('div');
            addMoreLink.className = 'add-more-link';
            addMoreLink.textContent = '+ Add More Parts';
            addMoreLink.addEventListener('click', addMoreParts);
            
            addMoreContainer.appendChild(addMoreLink);
            parentElement.appendChild(addMoreContainer);
        }
        
        // Function to add more parts
        function addMoreParts() {
            additionalPartsCounter++;
            const container = document.getElementById('additional-parts-container');
            
            const partGroup = document.createElement('div');
            partGroup.className = 'additional-part-group';
            partGroup.id = `additional-part-${additionalPartsCounter}`;
            
            // Create a heading for the additional part
            const heading = document.createElement('h4');
            heading.textContent = `Additional Part ${additionalPartsCounter}`;
            heading.style.marginTop = '0';
            partGroup.appendChild(heading);
            
            // Create Old Serial Number field
            const oldSerialGroup = document.createElement('div');
            oldSerialGroup.className = 'form-group';
            
            const oldSerialLabel = document.createElement('label');
            oldSerialLabel.setAttribute('for', `oldSerialNumber${additionalPartsCounter}`);
            oldSerialLabel.textContent = 'Old Serial Number';
            
            const oldSerialInput = document.createElement('input');
            oldSerialInput.type = 'text';
            oldSerialInput.id = `oldSerialNumber${additionalPartsCounter}`;
            oldSerialInput.name = `oldSerialNumber${additionalPartsCounter}`;
            oldSerialInput.addEventListener('input', updatePreview);
            
            oldSerialGroup.appendChild(oldSerialLabel);
            oldSerialGroup.appendChild(oldSerialInput);
            partGroup.appendChild(oldSerialGroup);
            
            // Create New Serial Number field
            const newSerialGroup = document.createElement('div');
            newSerialGroup.className = 'form-group';
            
            const newSerialLabel = document.createElement('label');
            newSerialLabel.setAttribute('for', `newSerialNumber${additionalPartsCounter}`);
            newSerialLabel.textContent = 'New Serial Number';
            
            const newSerialInput = document.createElement('input');
            newSerialInput.type = 'text';
            newSerialInput.id = `newSerialNumber${additionalPartsCounter}`;
            newSerialInput.name = `newSerialNumber${additionalPartsCounter}`;
            newSerialInput.addEventListener('input', updatePreview);
            
            newSerialGroup.appendChild(newSerialLabel);
            newSerialGroup.appendChild(newSerialInput);
            partGroup.appendChild(newSerialGroup);
            
            // Create License Plate field
            const licensePlateGroup = document.createElement('div');
            licensePlateGroup.className = 'form-group';
            
            const licensePlateLabel = document.createElement('label');
            licensePlateLabel.setAttribute('for', `licensePlate${additionalPartsCounter}`);
            licensePlateLabel.textContent = 'License Plate';
            
            const licensePlateInput = document.createElement('input');
            licensePlateInput.type = 'text';
            licensePlateInput.id = `licensePlate${additionalPartsCounter}`;
            licensePlateInput.name = `licensePlate${additionalPartsCounter}`;
            licensePlateInput.addEventListener('input', updatePreview);
            
            licensePlateGroup.appendChild(licensePlateLabel);
            licensePlateGroup.appendChild(licensePlateInput);
            partGroup.appendChild(licensePlateGroup);
            
            // Add Delete button with unique ID for better targeting
            const deleteButton = document.createElement('button');
            deleteButton.className = 'delete-group-btn';
            deleteButton.textContent = 'Delete this part';
            deleteButton.id = `delete-part-${additionalPartsCounter}`;
            deleteButton.setAttribute('type', 'button'); // Prevent form submission
            deleteButton.setAttribute('data-part-id', additionalPartsCounter);
            
            // Add click event with proper context
            deleteButton.onclick = function() {
                const partId = this.getAttribute('data-part-id');
                deletePartGroup(partId);
            };
            
            partGroup.appendChild(deleteButton);
            container.appendChild(partGroup);
            
            updatePreview();
            
            // Move the Add More button after the most recently added part
            addAddMoreButton(container);
        }
        
        // Function to ensure the Add More button is always last
        function ensureAddMoreButtonIsLast() {
            const addMoreContainer = document.getElementById('add-more-container');
            if (addMoreContainer) {
                const form = document.getElementById('template-form');
                form.appendChild(addMoreContainer);
            }
        }
        
        // Function to delete a part group
        function deletePartGroup(partId) {
            const partGroup = document.getElementById(`additional-part-${partId}`);
            if (partGroup) {
                partGroup.remove();
                updatePreview();
                ensureAddMoreButtonIsLast();
            }
        }
        
        // Function to check if conditional field should be shown
        function shouldShowConditionalField(field) {
            if (!field.conditionalOn) return true;
            
            const dependsOnField = document.getElementById(field.conditionalOn.field);
            return dependsOnField && dependsOnField.value === field.conditionalOn.value;
        }
        
        // Function to handle showing/hiding conditional fields
        function handleConditionalFields(event) {
            const triggerField = event.target;
            const triggerValue = triggerField.value;
            const conditionalFields = document.querySelectorAll(`.conditional-field[data-depends-on="${triggerField.id}"]`);
            
            conditionalFields.forEach(field => {
                const requiredValue = field.getAttribute('data-depends-value');
                if (triggerValue === requiredValue) {
                    field.style.display = 'block';
                } else {
                    field.style.display = 'none';
                    // Clear values in hidden fields
                    const inputs = field.querySelectorAll('input, textarea, select');
                    inputs.forEach(input => {
                        input.value = '';
                    });
                }
            });
            
            // Update preview after handling conditional fields
            updatePreview();
        }
        
        // Function to update preview as user types
        function updatePreview() {
            const formData = {};
            const template = templates[currentTemplate];
            
            // Collect values from regular fields
            template.fields.forEach(field => {
                const input = document.getElementById(field.name);
                if (input) {
                    formData[field.name] = input.value;
                }
            });
            
            // Collect values from additional parts
            if ((currentTemplate === 'breakfix' || currentTemplate === 'networking')) {
                formData.additionalParts = [];
                
                // Look for all additional parts in the DOM
                for (let i = 1; i <= additionalPartsCounter; i++) {
                    const partGroup = document.getElementById(`additional-part-${i}`);
                    if (partGroup) {
                        const oldSerial = document.getElementById(`oldSerialNumber${i}`);
                        const newSerial = document.getElementById(`newSerialNumber${i}`);
                        const licensePlate = document.getElementById(`licensePlate${i}`);
                        
                        if (oldSerial && newSerial && licensePlate) {
                            formData.additionalParts.push({
                                id: i,
                                oldSerialNumber: oldSerial.value,
                                newSerialNumber: newSerial.value,
                                licensePlate: licensePlate.value
                            });
                        }
                    }
                }
            }
            
            // Format the note with additional parts
            let formattedNote = template.format(formData);
            
            // Add additional parts info to the formatted note
            if ((currentTemplate === 'breakfix' || currentTemplate === 'networking') && formData.additionalParts && formData.additionalParts.length > 0) {
                formattedNote += '\n\nADDITIONAL PARTS:';
                
                formData.additionalParts.forEach((part, index) => {
                    formattedNote += `\n\nPART #${index + 2}:
OLD SERIAL NUMBER: ${part.oldSerialNumber || "N/A"}
NEW SERIAL NUMBER: ${part.newSerialNumber || "N/A"}
LICENSE PLATE: ${part.licensePlate || "N/A"}`;
                });
            }
            
            previewDiv.textContent = formattedNote;
        }
        
        // Complete button click handler
        completeBtn.addEventListener('click', () => {
            updatePreview(); // Ensure preview is current
            previewDiv.focus();
        });
        
        // Copy button click handler
        copyBtn.addEventListener('click', () => {
            const noteText = previewDiv.textContent;
            navigator.clipboard.writeText(noteText).then(() => {
                copyMessage.classList.add('show');
                setTimeout(() => {
                    copyMessage.classList.remove('show');
                }, 2000);
            });
        });
        
        // Reset button click handler
        resetBtn.addEventListener('click', () => {
            templateForm.reset();
            
            // Also reset any conditional fields
            const conditionalFields = document.querySelectorAll('.conditional-field');
            conditionalFields.forEach(field => {
                field.style.display = 'none';
            });
            
            // Remove any additional parts
            const additionalPartsContainer = document.getElementById('additional-parts-container');
            if (additionalPartsContainer) {
                additionalPartsContainer.innerHTML = '';
            }
            additionalPartsCounter = 0;
            
            // Reset the add more button position
            if (currentTemplate === 'breakfix' || currentTemplate === 'networking') {
                addAddMoreButton(templateForm);
            }
            
            updatePreview();
        });
    </script>
</body>
</html>
