Portfolio Entry: DemoVisualizationTMS

Description:
The DemoVisualizationTMS project is an AR-based system designed for real-time Transcranial Magnetic Stimulation (TMS) guidance using Magic Leap 1. The system is divided into two phases—registration and TMS targeting—and was developed as a simplified demo to quickly set up and deploy for demonstrations. This project showcases my expertise in AR development, spatial alignment, and user feedback mechanisms.

Phase 1: Registration

The user places markers (spheres) on specific fiducial points of the subject’s head to ensure accurate coil targeting later during TMS. This phase allows for flexible marker placement and adjustment. 

	•	Key Features:
	•	Markers are placed on key anatomical landmarks: inner ear, corner of the eye, nostril, and chin.
	•	The controller’s white sphere acts as an interactive pointer for marker placement.
	•	Users can delete markers if not satisfied with placement and reset the entire setup if needed.
	•	Controls:
	•	Trigger: Place marker.
	•	Bumper: Delete marker.
	•	Home button: Finalize registration or reset the scene.
	•	Skills Used:
	•	Unity (C#) for building the registration system with interactive controls.
	•	3D Spatial Mapping: Align markers with anatomical features using Magic Leap’s AR capabilities.

Phase 2: AR-guided TMS

This phase provides real-time feedback on the coil’s position relative to the subject’s skull. The coil is modeled as a 3D mesh, and the controller overlay guides placement. Visual feedback is provided to ensure accurate coil positioning based on a raycast from the controller to the subject’s brain.

	•	Key Features:
	•	The coil’s position is tracked using the Magic Leap controller, and a 3D mesh is overlaid on the controller for visual guidance.
	•	A raycast is shot from the coil’s centroid to the target brain region, and colored feedback dots appear at the point of intersection.
	•	The color gradient (blue to red) represents the accuracy of coil placement, with red indicating proximity to the target.
	•	Skills Used:
	•	Raycasting: Implemented to measure coil alignment and generate real-time feedback on the accuracy of placement.
	•	Real-time 3D Mesh Rendering: Overlay of the coil model for precise visual feedback.

Challenges and Solutions:

	•	Design Challenge: Simplifying complex spatial alignment for a quick and intuitive user interface.
	•	Solution: Developed a straightforward user interface where a white sphere guides the user to place fiducials at specific landmarks, with clear visual feedback controls.
	•	Feedback Mechanism: Needed a way to provide real-time, intuitive feedback on the coil’s placement.
	•	Solution: Integrated raycasting and color-coded visual cues (red for close, blue for far) to simplify the correction process.

Technologies:

	•	Unity (C#): Core development for AR-based interaction and interface.
	•	Magic Leap: Head-mounted display device used for AR visualization and real-world tracking.
	•	Raycasting: Used for spatial tracking and feedback based on coil positioning.
	•	3D Mesh Rendering: Overlay for TMS coil, allowing users to visualize alignment in real-time.

Outcomes:

	•	Created an easy-to-deploy demonstration tool for AR-guided TMS that highlights the potential for AR in medical applications.
	•	Improved User Interaction: Simplified user controls, allowing non-technical users to place fiducial markers and align TMS coils effectively.
	•	Visual Feedback: Integrated a user-friendly, color-coded feedback system to indicate the accuracy of coil placement in real-time.

Future Work:

	•	TCP Integration: Reintegrating real-time communication with Brain Vision software to visualize EEG/EMG data during TMS procedures.
	•	Enhancing Accuracy: Improving the tracking (OptiTrack system) and alignment algorithms to support clinical environments.
	•	Audio Feedback: Integrate audio feedback to guide coil placement.
	•	Upgrade for Magic Leap 2: Adapt the project for compatibility with Magic Leap 2.

How to Use:

	•	Place Markers: Align the controller with key landmarks (inner ear, eye corner, nostril, chin) and place markers using the trigger.
	•	Adjust Markers: If needed, delete misplaced markers using the bumper.
	•	TMS Targeting: Align the coil with the skull, shoot a raycast from the coil to the brain target, and observe the color-coded feedback and displayed metrics for positioning accuracy.
