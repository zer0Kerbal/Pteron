// changelog.md v1.0.0.0
// Pteron (PMSRV)
// created: 2020 02 25
// updated: 25 May 2021

# Changelog

| modName | Petreon (PMSRV!)                                               |
| ------- | -------------------------------------------------------------- |
| license | CC BY-NC-SA 4.0                                                            |
| website | https://forum.kerbalspaceprogram.com/index.php?/topic/191424-* |
| author  |  Sage Sagan and zer0Kerbal                     |

## Version 0.9.9.9-prerelease - See Clearly the Flames!

- 10 Jan 2022  
- Release for Kerbal Space Program [KSP 1.12.x] 

### parachutes

- adjusted drag
- closes #22

### [pmv-hydra]

- in order to have engine effects, had to remove multimode
- engine FX are now working
- one mode engine - same as afterburner
- added drag cube
- Elon Kermin found increased efficiency! and added an alternator
- closes #20

### <en-us.cfg>

- adjust to reflect changes
- manual lint and style
- closes #27
- updates #20

### Pteron.version

- change Changelog.cfg --> changelog.md
- update release version
- update minimum KSP version

### [pmv-engine]

- engine FX are now working #20
- Elon Kermin found increased efficiency!
  
### [pmv-dockingport]

- adjust [node_stack_bottom] y location
- adjust [node_stack_top] y location
- [ModuleDockingNode]: referenceAttachNode = bottom instead of top - this made it REALLY hard to dock!
- [description] from #pmv--dock-desc to #pmv-dock-desc (darn hyphen-monster again!)
- manual lint and style
- closes #13

### [pmv-shuttle-body]

- adjust [node_stack_bottom_APrt] y location
- adjust [node_stack_bottom_AStb] y location
- adjust [node_stack_bottom_BDsl] y location
- adjust [node_stack_bottom_BVnt] y location
- adjust [node_stack_gear] to make retracted gear flush

closes #14 - Version 0.9.9.9-prerelease
closes #15 - 0.9.9.9-prerelease Social 
closes #16 - 0.9.9.9-prerelease Release
closes #17 - 0.9.9.9-prerelease Update documentatio
closes #18 - 0.9.9.9-prerelease Legal MumboJumbo

## Version 0.9.0.0 - Pull in case of Emergency!

- 30 Jun 2021
- release for KSP 1.12.x

### [pmv-hydra]

- now uses new model with permission from artwhaley's Axial Aerospace Dreamer  
- added Alternator (only to this part)
- two mode engine - vacuum and afterburner

### add

- Restock whitelist patch (default off) thank you [@KawaiiLucy](https://forum.kerbalspaceprogram.com/index.php?/profile/201212-kawaiilucy/)  

### Add 

- drag cubes
- ModuleCargoPart
- defaultActionGroup = Gear

### [pmv-shuttle-body]

- ModuleResourceConverter
- ODFC.cfg v1.1.0.0
- add ModuleInventoryPart		
- InventorySlots = 6
- packedVolumeLimit = 2500

### adjust

- body node_stack_bottom = 0.0, -1.44456, 0.0, 0.0, -1.0, 0.0, 1, 1
- docking port 180z rotation
  - node_stack_bottom = 0.0, -0.20625, 0.0, 0.0, -1.0, 0.0, 1, 1, 1
  - node_stack_top = 0.0, 0.009, 0.001, 0.0, 1.0, 0.0, 1, 1
- WINGS
  - NODE ORIENTATION	

### Firespitter.cfg

- move Firespitter wheel module into patch
- use stock ModuleAnimateGeneric if Firespitter is not installed.

### [pmv-dockingport]

- ~~now uses new multi-light ModuleLight~~
- revert from multi-light, instead add color and blink to the two sets of lights.


# Version 0.8.0.0 - Pull in case of Emergency!

- 30 Jun 2021
- for KSP 1.12.1

- add engine to Restock whitelist (default off)
- add Restock patch (default is on)
        CHANGE {
            type = [Pmv-Hydra]
            change = now uses new model with permission from artwhaley's Axial Aerospace Dreamer  
            change = added Alternator (only to this part)
            change = two mode engine - vacuum and afterburner
        }

        CHANGE {
            type = Add
            change = Restock whitelist patch (default off) thank you [@KawaiiLucy](https://forum.kerbalspaceprogram.com/index.php?/profile/201212-kawaiilucy/)  
        }

        CHANGE {
            type = Add
            change = ModuleResourceConverter
        }

        CHANGE {
            type = Add
            change = On Demand Fuel Cells <ODFC.cfg v1.1.0.0>
        }

        CHANGE {
            type = Add
            change = drag cubes
            change = ModuleCargoPart
            change = defaultActionGroup = Gear
        }

        CHANGE {
            type = [Pmv-Shuttle-Body]
            change = add ModuleInventoryPart
            change = InventorySlots = 6
            change = packedVolumeLimit = 2500
        }

        CHANGE {
            type = Adjust
            change = body node_stack_bottom = 0.0, -1.44456, 0.0, 0.0, -1.0, 0.0, 1, 1
            change = docking port 180z rotation
            subchange = node_stack_bottom = 0.0, -0.20625, 0.0, 0.0, -1.0, 0.0, 1, 1, 1
            subchange = node_stack_top = 0.0, 0.009, 0.001, 0.0, 1.0, 0.0, 1, 1
        }

        CHANGE {
            type = Adjust
            change = WINGS
            subchange = NODE ORIENTATION	
        }

        CHANGE {
            type = Firespitter.Cfg
            change = move Firespitter wheel module into patch
            change = use stock ModuleAnimateGeneric if Firespitter is not installed.
        }

        CHANGE {
            type = [Pmv-Dockingport]
            change = ~~now uses new multi-light ModuleLight~~
            change = revert from multi-light, instead add color and blink to the two sets of lights.
        }
    }
	VERSION
	{
		version = 0.8.0.0
		versionName = <color=#ff0000><b>Chutes and Ladders</b></color>
		change = release for KSP 1.11.x
		change = add engine to Restock whitelist (default off)
		change = add Restock patch
		CHANGE
		{
			change = Added Firespitter.cfg patch
			subChange = moved Firespitter wheel code from wings and gear to patch
			subChange = replaced with ModuleAnimateGeneric
			subChange = this is only to address the boughts of altitude sickness and diziness from vessels spawning 1000 meters above the covers.
		}
		CHANGE
		{
			change = [pmv-engine] miniPuff 
			subChange = make it multi-mode
			subChange = add attachment node to top
			subchange = adjust attachment and bulkheadProfiles
		}
		CHANGE
		{
			change = wings and body
			subChange = add attachment nodes
		}
		CHANGE
		{
			change = add parts
			subChange = mini-RadialDrogue-rect
			subChange = mini-RadialDrogue-rnd
			subChange = mini-RadialChute-rect
			subChange = mini-RadialChute-rnd
		}
		change - Adjust pmv-shuttle-body CoMOffset (from 0.30 to 0.32) and CoLOffset (from 0.030 to 0.33)
	}
	VERSION
	{
		version = 0.7.0.0
		versionName =  Landing me softly
		change = RELEASE from pre-release
		change = adjusted FireSpitter FSWheel settings to try and soften landings
	}
	VERSION
	{
		version = 0.6.6.0
		versionName =  Right'round OverKill
		change = Thank you to @overkill13
		change = corrected numerous dyslexic keystrokes - verison -> version
		CHANGE
		{
			change = body
			subChange = adjust [ModuleControlSurface] deflectionLiftCoeff to 0.8 from 1.0
		}
		CHANGE
		{
			change = wings
			subChange = adjust [ModuleControlSurface] deflectionLiftCoeff to 0.8 from 1.0
		}
		CHANGE
		{
			change = suspension experiment (both wings and nose gear)
			subchange = added additional /optional/ module key nodes
			subchange = added (default value): overrideModelSpringValues = false;
			subchange = added (default value): overrideSuspensionDistance = false
			subchange = added (default value): forwardsStiffness = 10.0 // 3.0 // Forwards friction (Unity default is 1.0, which is not enough to get up small hills)
			subchange = added (default value): //forwardsStiffness = 10.0; // float //for tire friction
			subchange = added (default value): forwardsExtremumValue = 20000.0; // float
			subchange = added (default value): orwardsAsymptoteSlip = 2.0; // float
			subchange = added (default value): orwardsAsymptoteValue = 10000.0; // float
			subchange = added (default value): sidewaysStiffness = 1.0; // float //for tire friction
			subchange = added (default value): sidewaysExtremumSlip = 1.0; // float
			subchange = added (default value): sidewaysExtremumValue = 20000.0; // float
			subchange = added (default value): sidewaysAsymptoteSlip = 2.0; // float
			subchange = added (default value): sidewaysAsymptoteValue = 10000.0; // float
			subchange = added (default value): wheelColliderMass = -1; // float
			subchange = added (default value): wheelColliderRadius = -1; // float
			subchange = added (default value): wheelColliderSuspensionDistance = -1; // float
			subchange = added (default value): suspensionSpring = -1; // float
			subchange = added (default value): suspensionDamper = -1; // float
			subchange = added (default value): suspensionTargetPosition = -1; // float
		}
		CHANGE
		{
			change = right (port) wing only: 
			change = to address unholy asymetical heating difference between port/stbd wings
			subChange = increased maxTemp from 2000 to 2200
			subChange = increased skinMaxTemp from 2400 to 2500 (yes that is only 100° vs 200°)
		}
		CHANGE
		{
			change = dockingport
			subChange = reverted rotation to 0,0,0 from 180,0,0
			subChange = lowered resourceAmount from 0.18 to 0.04 
			subChange = reverted module changes (light issue)
		}
	}
	VERSION
	{
		version = 0.6.5.0
		versionName =  Head o'er Heals
		change = Thank you to @overkill13
		change = accepted PR from @overkill13
		change = cleaned out commented code
		CHANGE
		{
			change = body
			subChange = incoming changes from @Overkill's PR
			subChange = UNcommented out [ModuleLiftingSurface] :)
		}
		CHANGE
		{
			change = wings
			subChange = incoming changes from @Overkill's PR
		}
		CHANGE
		{
			change = dockingport
			subChange = reversed names of top/bottom nodes to fix 'Control from Here' issue
			subChange = attempting to get both sets of lights working
			subChange = split 'LightAnim" -> 'LightAniA' and 'LightAniB' in .mu
			subChange = put special sauce back in (uncommented in [ModuleDockingNode])
			subChange = added more Kyanoacrylate: breakingForce 200 -> 300
			subChange = added more Kyanoacrylate: breakingTorque 200 -> 300
		}
		CHANGE
		{
			change = PMV-nose-gear (SmallGearBay)
			subChange = added more Kyanoacrylate: breakingForce 150 -> 300
			subChange = added more Kyanoacrylate: breakingTorque 250 -> 300
			subChange = incoming changes from @Overkill's PR
		}
	}
	VERSION
	{
		version = 0.6.4.0
		versionName = Polishing the Mirrors
		change = Thank you to @overkill13
		CHANGE
		{
			change = body
			subChange = commented out CoMOffset change: 0.0, 0.0, 0.0 was 0.0, 0.0, 0.1
			subChange = CoLOffset change: 0.0, -0.1, 0.0 was 0.0, -0.5, 0.0
			subChange = commented out [ModuleLiftingSurface]
			subChange = deflectionLiftCoeff: to 2.5 from 1.85
			subChange = commented out DRAG_CUBE
			subChange = [ModuleRCSFX] shieldCanThrust changed to true from false
		}
		CHANGE
		{
			change = wings
			subChange = mismatched [RCSFX] thrusterPower (left was 0.75 right was 0.58) now both 0.75
			subChange = commented out [ModuleLiftingSurface]
			subChange = [ModuleControlSurface] ctrlSurfaceArea to 0.90 from 0.5
			subChange = commented out CoMOffset was 0.0, -0.5, 0
			subChange = changed CoLOffset to 0.0, -1.3, 0.0 from 0.0, -0.5, 0
			subChange = changed [ModuleControlSurface] deflectionLiftCoeff to 3.0 from 0.5
		}
		CHANGE
		{
			change = dockingport
			subChange = attempting to get both sets of lights working
			subChange = commented out DRAG_CUBE
		}
	}
	VERSION
	{
		version = 0.6.3.0
		versionName = Cleaning the Windows
		change = Thank you to @overkill13
		CHANGE
		{
			change = body
			subChange = CoMOffset change: 0.0, 0.0, 0.1 was 0.0, 0.0, 0.5
		}
		CHANGE
		{
			change = dockingport
			subChange = shift node_stack_bottom -Y from 0.2163243 to -0.2163243
			subChange = changed staged = false to true [ModuleDockingNode]
			subChange = commented out extraneous items [ModuleDockingNode]
			subChange = added back in stagingIcon
		}
		CHANGE
		{
			change = MiniOMS PMV-engine
			subChange = changed thrust from 4 to 4.5
			subChange = change vacuum ISP from 295 to 270 to remind it that its MP and inefficent. (same as it's big brother)
			subChange = [ModuleGimbal] gimbalRange bumped from 1 to 3 (1/4 of full scale)
			subChange = [ModuleGimbal] commented out gimbalResponseSpeed and useGimbalResponseSpeed (don't know if #'s higher better or worse)
			subChange = to reflect increased thrust: changed rescaleFactor from .25 to .33
			subChange = to reflect increased size: increased mass from 0.02 to 0.025
		}
		CHANGE
		{
			change = PMV-nose-gear (SmallGearBay)
			subChange = re-add skinMaxTemp = 2700 - hopefully it sticks this time
			subChange = removed weird appendix attachRules = 1,1,1,1,1,0,0,0????
			subChange = removed DRAG_CUBE to see if that helps with it sleeping THIS far above the covers
		}
		CHANGE
		{
			change = wings
			subChange = commented out KSP calc DRAG_CUBE
			subChange = change ctrlSurfaceArea to 0.5  from 0.78 *
			subChange = change dragCoeff to 0.5 from 0.3 *
			subChange = toggle deploy to false
			subChange = * : from 0.5.0.0 version
		}
	}
	VERSION
	{
		version = 0.6.2.0
		versionName = Brushing off the Construction Dust
		change = Thank you to @overkill13
		CHANGE
		{
			change = wings
			subChange = ModuleLiftingSurface (deflectionLiftCoeff = 2.0 was 5.0)
			subChange = ModuleControlSurface (ctrlSurfaceArea = 0.5 was 0.78)
			subChange = added: CoMOffset = 0.0, -0.5, 0
			subChange = added: CoLOffset = 0.0, -0.5, 0
		}
		CHANGE
		{
			change = body
			subChange = ModuleLiftingSurface (deflectionLiftCoeff = 1.85 was 5.0)
			subChange = CoMOffset change: 0.0, 0.0, 0.5 was 0.0, 0.8, 0.0
			subChange = CoLOffset change: 0.0, -0.5, 0.0 was 0.0, -1.5, 0.0
		}
	}

## Version 0.6.1.0 - Brushing off the Construction Dust

-  Thank you to @overkill13
-  apologies, forgot to include Firespitter as a required mod (wheels)
-  adjusted CoM +y
-  adjusted CoL +z
-  fix attachement for MiniOMS engines
-  fix decoupler node on docking port
-  max temps on wings different - gave them the same haircut
-  R/W on body from 5/3/3 to 5/-
-  controlpoint noseup20 to nosedown15
-  body skinMaxTemp from 2700 -> 2200
-  wings skinMaxTemp from 2700/2500 -> 2400
-  wings maxTemp from 2400 -> 2000
-  added breakeringForce/Torque 200 to docking port
-  dockingport referenceAttachNode changed from top to bottom
-  dockingport staged changed to false, still can enable

## Version 0.6.0.0 -  Brushing off the Construction Dust

- >>-- adopted for curation by @zer0Kerbal --<<

### organize for adoption
- folder structure
- added license(s) file(s)
- added .version file
- Readme
- automated backend
- jsons
- Changelog.md -> Kerbal Changelog Changelog.cfg
- updated Readme.md
- moved changelog into separate file
		}
		CHANGE
		{
			change = Online
			subChange = GitHub Repo
			subChange = created Forum Thread
			subChange = updated SpaceDock
			subChange = updated CKAN/NetKAN
		}
		CHANGE
		{
			change = modernization, polish, update pass on .cfg
			subChange = large .tga -> .dds (9.5mb -> 7.0mb)
			subChange = - replaced mesh = with MODEL{}
			subChange = merged in patches
			subChange = updated from RCS -> RCSFX
			subChange = added EFFECTS RCSFX
			subChange = updated ModuleCommand
			subChange = updated ModuleSAS
			subChange = updated ModuleReactionWheel (what level??)
			subChange = lowered EC/consumption from 0.2 -) 0.04
			subChange = updated ModuleScienceExperiment
			subChange = updated ModuleScienceContainer
			subChange = replaced ModuleGenerator -> ModuleResourceConverter
			subChange = added ODFC.cfg patch, with following scaling patch (*see if it works*)
			subChange = ModuleLight (EC/s from 0.18 -> 0.04) lightBrightenSpeed from 2 -> 2.5
			subChange = dropped MonoPropellant from 250 to 50 (still might be too high?)
			subChange = dropped ElectricCharge from 180 to 100 (still might be too much?)
			subChange = moved dockingport from utility to coupling
			subChange = added bulkheadProfiles = size1
			subChange = added explosionPotential = 0.5
			subChange = moved nosegear from Utility to Ground
			subChange = changed PART module = wing to Part
			subChange = added MiniOMS MonoPropellant Engine
			subChange = adjusted and renamed nodes, added node_attach
			subChange = docking port - added 180° rotation (it was upside down)
			subChange = added tags = pteron
			subChange = added NEAR-Far.cfg patch, commented out FARWingAerodynamicModel's in wings 
		}
		CHANGE
		{
			change = PMV-shuttle-body (body) (mk3Cockpit_Shuttle)
			subChange = maximum_drag = 0.2 (mk3Cockpit_Shuttle = 0.1)
			subChange = minimum_drag = 0.15 (mk3Cockpit_Shuttle = 0.1)
			subChange = angularDrag = 2 (mk3Cockpit_Shuttle = 2)
			subChange = crashTolerance 50 (mk3Cockpit_Shuttle = 40)
			subChange = maxTemp = 1500 (mk3Cockpit_Shuttle = 1500)
			subChange = add skinMaxTemp = 2700  (mk3Cockpit_Shuttle = 2700)
			subChange = emissiveConstant = 0.9
			subChange = breakingForce from 50 to 300 (mk3Cockpit_Shuttle = 300)
			subChange = breakingTorque from 85 to 300 (mk3Cockpit_Shuttle = 300)
			subChange = [EXPERIMENTAL] added Nose Up Control Point (20°)
			subChange = [EXPERIMENTAL] added Nose Up Control Point (15°)
			subChange = vesselType from Ship to Plane
			subChange = added ModuleDataTransmitter 16S INTERNAL 100,000 (too much?)
			subChange = added localization
			subChange = added stagingIcon
			subChange = updated from RCS -> RCSFX
			subChange = added EFFECTS RCSFX
		}
		CHANGE
		{
			change = PMV-nose-gear (SmallGearBay)
			subChange = adjusted mass = 0.1 -> 0.05 (SmallGearBay = 0.45)
			subChange = adjusted maxTemp = from 3600 t0 2600 (SmallGearBay = 2600)
			subChange = add skinMaxTemp = 2700  (SmallGearBay = 2700)
			subChange = add thermalMassModifier = 4.0 
			subChange = add // heatConductivity = 0.06
			subChange = add emissiveConstant = 0.95
			subChange = adjusted crashTolerance 200 -> 50 (SmallGearBay = 50)
			subChange = note: breakingForce 150 (SmallGearBay = 50)
			subChange = note: breakingTorque 250 (SmallGearBay = 50)
			subChange = added localization
			subChange = added effect: deploy/deployed
			subChange = added effect: retract/retracted
			subChange = adjusted attachRules = 1,0,0,0,1 -> attachRules = 1,1,1,1,1,0,0,0????
			subChange = remove duplicate attachRules
			subChange = added ModuleDragModifier (Deployed/Restracted)
			subChange = added sFX (Deployed/Restracted)
		}
		CHANGE
		{
			change = PMV-dockingport (dockingPort2)
			subChange = adjust maxTemp 3400 -> 2000 (dockingPort2 = 2000)
			subChange = add stagingIcon = DECOUPLER_VERT
			subChange = add childStageOffset = 0
			subChange = updated ModuleDockingNode
		}
		CHANGE
		{
			change = PMV-wing-left/PMV-wing-right (wingShuttleDelta)
			subChange = Added for possible future use: // CoMOffset = -1.6, -0.4, 0
			subChange = Added for possible future use: // CoLOffset = -1.6, -0.4, 0
			subChange = Added for possible future use: // CoPOffset = -1.6, -0.4, 0
			aubChange = added thermalMassModifier = 8.0
			aubChange = added heatConductivity = 0.06 // half default
			aubChange = added emissiveConstant = 0.95
			aubChange = added dragModelType = override (wingShuttleDelta = none) ???
			aubChange = adjusted maxTemp = 3600 -> 2400 (wingShuttleDelta = 2400)
			aubChange = added 	skinMaxTemp = 2700
			aubChange = adjusted crashTolerance = 200 -> 15 (wingShuttleDelta = 15)
			aubChange = noted: breakingForce = 150 (wingShuttleDelta = none)
			aubChange = noted: breakingTorque = 250 (wingShuttleDelta = none)
			aubChange = added: ModuleLiftingSurface from wingShuttleDelta ???
			aubChange = added: MonoPropellant = 10
			aubChange = added ModuleDragModifier (Deployed/Restracted)
			aubChange = added sFX (Deployed/Restracted)
			aubChange = updated from RCS -> RCSFX
			aubChange = added EFFECTS RCSFX
			subChange = added stagingIcon
		}
		change = zer0Kerbal played with one of his mods
		change = added /Localization/
		change = added localization (en-us.cfg)
		change = adjusted phrasing a smudge
		change = moved art into Pteron/Assets/
		change = updated texture pointers in model (original, png, dds included)
		change = updated part.cfg:
		change = - added explosionPotential
		change = created Changelog.cfg [KERBALCHANGELOG] (.this)
		change = added additional fields in .version (might need to tweak urls)
		change = added shields to Readme.md
		change = adjusted nodes (flipped orientation as needed)
		
### Adoption by zer0Kerbal

- Send Adoption Papers
- Post Adoption Notice
- gather
- verify licenses
- look for existing repo/postings
	
## Version 0.5.0.0 - the pre-adoption partyBeta

- Beta Release 09/09/2014
- from original forum post's dropbox link

<!--- CC BY-ND 3.0 unported 2021 by zer0Kerbal-->