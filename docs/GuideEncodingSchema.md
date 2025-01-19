# Guide Encoding Schema

## Overview
This document is intended as a reference for the XML encoding schema for ironman efficiency guides in the Efficient BTW RuneLite plugin.

## Table of Contents
- [Guide](#guide)
- [Sections](#sections)
- [Section](#section)
- [Subsections](#subsections)
- [Subsection](#subsection)
- [Steps](#steps)
- [Step](#step)
- [ItemStep](#itemstep)
- [GpStep](#gpstep)
- [NpcStep](#npcstep)


## Guide
**Description:** The overall guide element.

**Parent Element:** None

**Child Elements:**
- [Sections](#sections)


## Sections
**Description:** The sections within the guide.

**Parent Element:** [Guide](#guide)

**Child Elements:** 
- [Section](#section)


## Section
**Description:** An individual section within the guide.

**Parent Element:** [Sections](#sections)

**Child Elements:**
- [Subsections](#subsections)


## Subsections
**Descriptions:** The subsections within a section of the guide.

**Parent Element:** [Section](#section)

**Child Elements:**
- [Subsection](#subsection)


## Subsection
**Descriptions:** An individual subsection within a section of the guide.

**Parent Element:** [Subsections](#subsections)

**Child Elements:**
- [Steps](#steps)


## Steps
**Descriptions:** The steps within a subsection of the guide.

**Parent Element:** [Subsection](#subsection)

**Child Elements:**
- [Step](#step)
- [ItemStep](#itemstep)
- [GpStep](#gpstep)
- [NpcStep](#npcstep)


## Step
**Descriptions:** An individual generic step within a subsection of the guide.

**Parent Element:** [Steps](#steps)

**Child Elements:** None

**Fields:**
| Field Name | Description | Required |
|------------|-------------|-----------|
| description | The description of the step to display to the user | Yes |
| completed | Boolean value (true/false) for whether the step has already been completed | No |
---


## ItemStep
**Descriptions:** An individual step within a subsection of the guide that deals with an item.

**Parent Element:** [Steps](#steps)

**Child Elements:** None

**Fields:**
| Field Name | Description | Required |
|------------|-------------|-------------|
| description | The description of the step to display to the user | Yes |
| item_name | The name of the item | Yes |
| item_id | The item ID | No |
| drop | Boolean value (true/false) for whether the item should be dropped; defaults to false | No |
| completed | Boolean value (true/false) for whether the step has already been completed | No |
---


## GpStep
**Descriptions:** An individual step within a subsection of the guide that deals with GP.

**Parent Element:** [Steps](#steps)

**Child Elements:** None

**Fields:**
| Field Name | Description | Required |
|------------|-------------|-------------|
| description | The description of the step to display to the user; information on where to obtain the GP can be included here | Yes |
| gp_amount | The amount of GP required for the step | Yes |
| completed | Boolean value (true/false) for whether the step has already been completed | No |
---


## NpcStep
**Descriptions:** An individual step within a subsection of the guide that deals with an NPC.

**Parent Element:** [Steps](#steps)

**Child Elements:** None

**Fields:**
| Field Name | Description | Required |
|------------|-------------|-------------|
| description | The description of the step to display to the user | Yes |
| npc_name | The name of the NPC | Yes |
| npc_location | The location of the NPC | Yes |
| kill | Boolean value (true/false) for whether the the NPC should be killed; defaults to false (talk to) | No |
| completed | Boolean value (true/false) for whether the step has already been completed | No |
---






## 
**Descriptions:** 

**Parent Element:** []()

**Child Elements:**
- []()

**Fields:**
| Field Name | Description | Required |
|------------|-------------|-------------|
| Name | Description of the Name field | Yes |
| Value | Description of the Value field | |
---