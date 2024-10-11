Portfolio Entry: DemoVisualizationTMS

Description:
The DemoVisualizationTMS project is an AR-based system designed for real-time Transcranial Magnetic Stimulation (TMS) guidance using Magic Leap 1. The system is divided into two phases—registration and TMS targeting—and was developed as a simplified demo for quick deployment and setup in demonstration contexts. This project showcases my expertise in AR development, spatial alignment, and user feedback mechanisms.

Phase 1: Registration

The user places markers (spheres) on specific fiducial points of the subject’s head to ensure accurate coil targeting later during the TMS procedure. This phase allows for flexible marker placement and adjustment.

	•	Key Features:
	•	Markers are placed on key anatomical landmarks: inner ear, corner of the eye, nostril, and chin.
	•	The controller’s white sphere acts as an interactive pointer for marker placement.
	•	Users can delete markers if not satisfied with placement and reset the entire setup if needed.
	•	Controls:
	•	Trigger: Place marker.
	•	Bumper: Delete marker.
	•	Home button: Finalize registration or reset the scene.
	•	Skills Used:
	•	Unity (C#) for developing the registration system with interactive controls.
	•	3D Spatial Mapping: Align markers with anatomical features using Magic Leap’s AR capabilities.

Phase 2: AR-guided TMS

In this phase, real-time feedback is provided on the coil’s position relative to the subject’s skull. The coil is represented by a 3D mesh, and the controller’s overlay guides the user in positioning it. Visual feedback is provided to ensure accurate coil placement based on a raycast from the controller to the subject’s brain.

	•	Key Features:
	•	The coil’s position is tracked using the Magic Leap controller, with a 3D mesh overlay providing visual guidance.
	•	A raycast is shot from the coil’s centroid to the target brain region, with colored feedback dots appearing at the point of intersection.
	•	A color gradient (blue to red) represents the accuracy of coil placement, with red indicating proximity to the target.
	•	Skills Used:
	•	Raycasting: Used to measure coil alignment and generate real-time feedback on the accuracy of placement.
	•	Real-time 3D Mesh Rendering: Displayed the coil model for precise visual feedback.

Challenges and Solutions:

	•	Design Challenge: Simplifying complex spatial alignment for a quick and intuitive user interface.
	•	Solution: Developed a user interface where a white sphere guides users to place fiducials at specific landmarks, with clear visual feedback controls.
	•	Feedback Mechanism: Needed a real-time, intuitive feedback system for coil placement accuracy.
	•	Solution: Integrated raycasting and color-coded visual cues (red for closer, blue for farther) to simplify the correction process and help users achieve optimal coil placement.

Technologies:

	•	Unity (C#): Core development for AR-based interaction and interface.
	•	Magic Leap: Head-mounted display device used for AR visualization and real-world tracking.
	•	Raycasting: Implemented for spatial tracking and accuracy feedback during coil positioning.
	•	3D Mesh Rendering: Enabled users to visualize the alignment of the TMS coil in real time.

Outcomes:

	•	Developed an easy-to-deploy demo tool for AR-guided TMS, highlighting the potential for AR in medical applications.
	•	Improved User Interaction: Simplified controls allowed non-technical users to place fiducial markers and align TMS coils effectively.
	•	Visual Feedback: Integrated a user-friendly, color-coded feedback system that indicates coil placement accuracy in real-time, improving precision and ease of use.

Future Work:

	•	TCP Integration: Reintegrating real-time communication with Brain Vision software to visualize EEG/EMG data during TMS procedures.
	•	Enhancing Accuracy: Improving the tracking system (OptiTrack) and alignment algorithms for use in clinical environments.
	•	Audio Feedback: Adding audio-based feedback to guide coil placement more effectively.
	•	Recording Capabilities: Reintegrating recording functionalities for retrospective analysis of accuracy and user learning curves.
	•	Magic Leap 2 Support: Upgrading the project for compatibility with Magic Leap 2 for enhanced AR capabilities.

How to Use:

	•	Place Markers: Align the controller with key landmarks (inner ear, eye corner, nostril, chin) and place markers using the trigger.
	•	Adjust Markers: Delete misplaced markers with the bumper, if needed.
	•	TMS Targeting: Align the coil with the skull, shoot a raycast from the coil to the brain target, and observe the color-coded feedback and displayed metrics for positioning accuracy.
