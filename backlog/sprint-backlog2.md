1. **Review Sprint 1 Deliverables**
 - 1.1 - Review strategic BPMN: Review the strategic BPMN model created in Sprint 1.
 - 1.2 - Review business processes: Check the identified business processes and their relationships.
 - 1.3 - Confirm major functionalities: Confirm the two major functionalities agreed by the group.
 - 1.4 - Review stakeholders: Check the actors and organisational responsibilities identified in Sprint 1.
 - 1.5 - Identify missing information: Identify gaps, assumptions or uncertainties that may affect further modelling.
 - 1.6 - Confirm Sprint 2 scope: Agree on the modelling and automation work to be completed during Sprint 2.

 2. **Create the i* Strategic Dependency (SD) Model**
 - 2.1 - Identify strategic actors: Identify the main stakeholders and organisational actors involved in the enterprise.
 - 2.2 - Define actor responsibilities: Establish the responsibilities and roles of each actor.
 - 2.3 - Identify actor goals: Identify the goals that each actor wants to achieve.
 - 2.4 - Identify goal dependencies: Identify goals that one actor depends on another actor to achieve.
 - 2.5 - Identify task dependencies: Identify tasks that one actor depends on another actor to perform.
 - 2.6 - Identify resource dependencies: Identify information, resources or services that actors depend on other actors to provide.
 - 2.7 - Identify relevant soft goals: Identify relevant quality expectations, such as reliability or usability.
 - 2.8 - Connect dependencies to functionalities: Relate the identified dependencies to the two agreed major functionalities.
 - 2.9 - Draw the initial SD model: Represent the actors and dependencies using the agreed i* notation.
 - 2.10 - Validate actor relationships: Check that the relationships reflect the case study and the group's analysis.
 - 2.11 - Review and correct the model: Identify missing actors or dependencies and make the necessary corrections.
 - 2.12 - Finalise the SD model: Save the completed model and supporting documentation in GitHub.

3. **Create the i* Strategic Rationale (SR) Model**
 - 3.1 - Review strategic actors: Use the actors identified in the SD model as the starting point for the SR model.
 - 3.2 - Identify actor goals: Define the main goals that each relevant actor wants to achieve.
 - 3.3 - Decompose goals: Break down high-level goals into smaller goals where appropriate.
 - 3.4 - Identify actor tasks: Identify the tasks each actor can perform to achieve their goals.
 - 3.5 - Identify required resources: Identify the information, resources or services needed to perform the tasks.
 - 3.6 - Identify soft goals: Identify relevant quality expectations that influence how goals should be achieved.
 - 3.7 - Connect goals and tasks: Show how tasks contribute to achieving specific goals.
 - 3.8 - Identify alternative approaches: Represent alternative ways of achieving goals where relevant.
 - 3.9 - Relate rationale to functionalities: Connect the goals and tasks to the two agreed major functionalities.
 - 3.10 - Draw the initial SR model: Represent the goals, tasks, resources and relationships using the agreed i* notation.
 - 3.11 - Check consistency with SD: Ensure that the SR model is consistent with the actors and dependencies in the SD model.
 - 3.12 - Review and correct the model: Resolve missing relationships, unclear elements or inconsistencies.
 - 3.13 - Finalise the SR model: Save the completed model and supporting documentation in GitHub.

4. **Develop Operational BPMN Model 1 — Producer Product Listing and Inventory Management**
 - 4.1 - Identify process participants: Identify the producer, marketplace system and any external verification service involved.
 - 4.2 - Define the start event: Identify the event that starts the product listing process.
 - 4.3 - Model product information entry: Represent the producer entering the product name, description, category, price and available quantity
 - 4.4 - Include additional product information: Account for farm origin, availability period, harvest date, allergen details, organic certification and best-before date where applicable.
 - 4.5 - Model information validation: Represent the system checking whether the required product information is valid.
 - 4.6 - Add the validation gateway: Add a gateway to separate valid submissions from submissions containing missing or invalid information.
 - 4.7 - Model correction of invalid information: Represent the system requesting corrections and the producer resubmitting the information.
 - 4.8 - Model certification verification: Include verification of organic certification when a producer makes an organic claim.
 - 4.9 - Model verification failure: Represent what happens if certification cannot be verified or the external service is unavailable.
 - 4.10 - Model product publication: Represent publication after the required checks have been completed successfully.
 - 4.11 - Model inventory updates: Represent the producer updating product quantities and seasonal availability.
 - 4.12 - Model stock depletion: Include the behaviour that makes a product unavailable when its stock reaches zero.
 - 4.13 - Model stock replenishment: Include the behaviour that allows a product to become available again when stock is replenished and the seasonal period remains valid.
 - 4.14 - Define end events: Identify the possible outcomes and appropriate end events for the process.
 - 4.15 - Validate BPMN notation: Check gateways, sequence flows, events, activities and participant boundaries.
 - 4.16 - Review against the use case: Confirm that the model represents the requirements and exception scenarios in the original use case.
 - 4.17 - Finalise the operational model: Save the completed BPMN model in GitHub.

5. **Develop Operational BPMN Model 2 — Second Major Functionality**
 - 5.1 - Confirm the second functionality: Identify the second major functionality agreed by the group.
 - 5.2 - Review the second use case: Examine the requirements, expected outcomes and relevant business rules.
 - 5.3 - Identify process participants: Identify the actors, systems and external services involved.
 - 5.4 - Define the start event: Identify what triggers the operational process.
 - 5.5 - Identify operational activities: Break down the use case into the individual tasks required to complete the process.
 - 5.6 - Identify decision points: Identify conditions that affect the process flow.
 - 5.7 - Add gateways: Represent the decision points using appropriate BPMN gateways.
 - 5.8 - Define sequence flows: Connect the activities and gateways in the correct execution order.
 - 5.9 - Model exception scenarios: Represent relevant failures, invalid inputs or alternative outcomes.
 - 5.10 - Define end events: Identify how and when the process can finish.
 - 5.11 - Validate the model: Check the model against the second use case and its business rules.
 - 5.12 - Finalise the operational model: Save the completed BPMN model in GitHub.

6. **Establish Traceability Between the Models**
 - 6.1 - Review i* model goals: Identify the relevant actor goals and dependencies in the SD and SR models.
 - 6.2 - Identify strategic processes: Identify the strategic BPMN processes that relate to the goals and dependencies.
 - 6.3 - Map strategic activities: Connect relevant activities in the strategic BPMN model to the detailed operational BPMN models.
 - 6.4 - Map goals to operational tasks: Identify which operational activities contribute to the goals represented in the i* models.
 - 6.5 - Check actor consistency: Ensure that actor responsibilities are consistent across all models.
 - 6.6 - Identify traceability gaps: Identify goals, dependencies or activities that are not represented consistently.
 - 6.7 - Correct inconsistencies: Update the relevant models to resolve identified gaps.
 - 6.8 - Create a traceability table: Document the relationships between the i* models, strategic BPMN and operational BPMN models.
 - 6.9 - Review traceability: Check that the relationships are understandable and supported by the models.
 - 6.10 - Save traceability evidence: Commit the traceability table and updated models to GitHub.

7. **Set Up Initial Executable Camunda Processes**
 - 7.1 - Confirm Camunda environment: Establish which Camunda version and execution environment the group will use.
 - 7.2 - Review execution requirements: Identify the configuration and implementation requirements for deploying executable BPMN processes.
 - 7.3 - Select an initial workflow: Choose a suitable workflow to implement first, considering dependencies and available time.
 - 7.4 - Create the process definition: Create the initial Camunda process based on the corresponding operational BPMN model.
 - 7.5 - Configure start and end events: Configure the events needed to initiate and finish the executable process.
 - 7.6 - Configure sequence flows: Connect the process activities in the intended execution order.
 - 7.7 - Configure gateways: Add gateways and define the conditions that determine which path the process follows.
 - 7.8 - Check model consistency: Confirm that the executable process reflects the agreed operational BPMN model.
 - 7.9 - Deploy the process: Deploy the initial process definition to the group's Camunda environment.
 - 7.10 - Execute a process instance: Start a process instance to check that the deployed process can run.
 - 7.11 - Resolve initial execution issues: Identify and fix basic deployment or execution errors.

8. **Implement Camunda User Tasks and Forms**
 - 8.1 - Identify user interaction points: Identify operational activities that require a person to enter information or make a decision.
 - 8.2 - Select initial user tasks: Choose the user tasks to implement during Sprint 2.
 - 8.3 - Configure user tasks: Add the selected user tasks to the executable Camunda processes.
 - 8.4 - Identify form requirements: Determine what information each user needs to enter or review.
 - 8.5 - Create initial forms: Create the forms required for the selected user tasks using the approach supported by the group's Camunda environment.
 - 8.6 - Add required form fields: Include the relevant input fields for each task.
 - 8.7 - Configure basic validation: Configure required fields and suitable input checks where supported.
 - 8.8 - Connect forms to process variables: Ensure that submitted form information is available to the process.
 - 8.9 - Test task completion: Confirm that users can access and complete the configured tasks.
 - 8.10 - Test form submissions: Check that submitted information is passed into the process correctly.

9. **Implement Initial Service Tasks**
 - 9.1 - Identify automation opportunities: Identify operational activities that can be automated without direct user interaction.
 - 9.2 - Select service tasks: Choose suitable activities for initial service-task implementation.
 - 9.3 - Define task inputs and outputs: Identify the information each selected service task requires and produces.
 - 9.4 - Implement initial service logic: Write the initial automation logic using the method supported by the group's Camunda environment.
 - 9.5 - Implement validation logic: Implement relevant automated checks where appropriate.
 - 9.6 - Implement business rules: Add the business logic needed for the selected automated activities.
 - 9.7 - Connect service tasks: Configure the process to execute the service-task implementation.
 - 9.8 - Handle unsuccessful outcomes: Account for relevant errors or unsuccessful results.
 - 9.9 - Test service tasks: Execute the service tasks with representative input data and check their outputs.
 - 9.10 - Document limitations: Record incomplete automation and any remaining dependencies.

10. **Configure Process Variables, Gateways and Business Logic**
 - 10.1 - Identify required process data: Determine what information must be retained throughout process execution.
 - 10.2 - Define process variables: Identify the required process variables and their intended data types.
 - 10.3 - Configure process variables: Add the variables required by the selected executable processes.
 - 10.4 - Pass form data into variables: Ensure that user-submitted information is stored in the appropriate variables.
 - 10.5 - Define gateway conditions: Determine the conditions that control the outgoing paths of the gateways.
 - 10.6 - Implement decision logic: Configure the relevant business rules that determine process behaviour.
 - 10.7 = Test valid inputs: Check that valid information leads to the expected process path.
 - 10.8 - Test invalid inputs: Check that invalid or missing information is handled appropriately.
 - 10.9 - Test gateway outcomes: Confirm that each implemented gateway follows the correct path for the tested conditions.
 - 10.10 - Document process logic: Record the variables, gateway conditions and business rules implemented.

11. **Test and Validate Initial Camunda Processes**
 - 11.1 - Define test scenarios: Identify normal, alternative and error scenarios for the implemented processes.
 - 11.2 - Test the normal process flow: Execute the process using valid input data.
 - 11.3 - Test gateway branches: Check that the process follows the expected paths for different conditions.
 - 11.4 - Test user tasks: Confirm that user tasks can be accessed and completed.
 - 11.5 - Test forms: Confirm that forms accept the expected inputs and submit data correctly.#
 - 11.6 - Test process variables: Check that process data is stored and passed between activities correctly.
 - 11.7 - Test service tasks: Check that the selected automated activities execute and return the expected results.
 - 11.8 - Test exception handling: Check the implemented behaviour for relevant failures and invalid inputs.
 - 11.9 - Compare execution with BPMN: Confirm that the executable process follows the intended operational workflow.
 - 11.10 - Record defects: Document unexpected behaviour and any failed test scenarios.
 - 11.11 - Resolve identified issues: Fix the issues that can reasonably be addressed during Sprint 2.
 - 11.12 - Record test evidence: Save test results and relevant evidence in the project repository.

12. **Maintain GitHub and Track Group Contributions**
 - 12.2 - Organise project files: Create or update folders for i* models, BPMN models, Camunda processes and supporting documentation.
 - 12.3 - Commit i* models: Commit the completed SD and SR models to GitHub.
 - 12.4 - Commit operational BPMN models: Commit both operational BPMN models and their latest revisions.#
 - 12.5 - Commit traceability documentation: Commit the traceability table and related documentation.
 - 12.6 - Commit Camunda implementation: Commit the initial process definitions and relevant implementation files.
 - 12.7 - Use meaningful commit messages: Ensure commit messages clearly describe the changes made.
 - 12.8 - Track issues and progress: Record outstanding tasks, defects and blockers using GitHub Issues or the group's agreed tracking method.
 - 12.9 - Record group decisions: Document agreed actions and decisions from meetings.
 - 12.10 - Review contributions: Check that each member's work and contributions are visible in the repository and task tracker.
 - 12.11 - Verify repository completeness: Confirm that the latest agreed models, code and evidence are committed and organised.

13. **Review Sprint 2 Deliverables**
 - 13.1 - Review the SD model: Confirm that the i* Strategic Dependency model is complete.
 - 13.2 - Review the SR model: Confirm that the i* Strategic Rationale model is complete.
 - 13.3 - Review operational BPMN model 1: Check that the product listing and inventory workflow is modelled in sufficient detail.
 - 13.4 - Review operational BPMN model 2: Check that the second agreed functionality is modelled in sufficient detail.
 - 13.5 - Review model traceability: Confirm that traceability between the i* models and the strategic and operational BPMN models is documented.
 - 13.6 - Review Camunda execution: Confirm that the initial executable process or processes can be deployed and run.
 - 13.7 - Review user tasks and forms: Check that the implemented user tasks and forms function as intended.
 - 13.8 - Review service-task implementation: Confirm that suitable initial service tasks have been implemented where appropriate.
 - 13.9 - Review variables and gateways: Check that process variables, gateway conditions and business logic work as intended.
 - 13.10 - Review test evidence: Check that testing results and known issues are documented.
 - 13.11 - Review GitHub contributions: Confirm that the repository demonstrates continued group development and collaboration.
 - 13.12 - Identify outstanding work: Record incomplete tasks, reasons for delays and priorities for the next sprint.
