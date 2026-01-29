# Pixel Blade - Architecture Overview

## System Architecture

This document provides an overview of the Pixel Blade architecture for Roblox scripting and automation.

```mermaid
graph TB
    subgraph "Execution Layer"
        EXE["Executors<br/>(Delta, Mobile, PC)"]
    end
    
    subgraph "Script Core"
        KB["Keyless Execution<br/>Module"]
        KA["Kill Aura<br/>System"]
        AF["Auto Farm<br/>System"]
        MU["Max Upgrades<br/>System"]
    end
    
    subgraph "UI/Frontend"
        HTML["HTML Interface<br/>(40.1%)"]
        CSS["CSS Styling<br/>(50%)"]
    end
    
    subgraph "Business Logic"
        JS["JavaScript Engine<br/>(9.9%)"]
        OPT["Optimization<br/>Module"]
    end
    
    subgraph "Features"
        SAFE["Safe Progression"]
        FAST["Fast Execution"]
        AUTO["Abilities Automation"]
    end
    
    EXE -->|Loads| KB
    KB -->|Initializes| JS
    JS -->|Manages| KA
    JS -->|Manages| AF
    JS -->|Manages| MU
    HTML -->|Renders| CSS
    JS -->|Controls| HTML
    OPT -->|Optimizes| JS
    KA -->|Enables| AUTO
    AF -->|Ensures| SAFE
    AF -->|Provides| FAST
    MU -->|Supports| AUTO
```

## Component Overview

### Execution Layer
- **Executors**: Compatible with Delta executor and mobile/PC executors
- Handles keyless execution for seamless script loading

### Script Core Modules

#### 1. **Kill Aura System**
   - Automated combat targeting and strikes
   - Safe operation without detection
   - Optimized for all executor types

#### 2. **Auto Farm System**
   - Automated resource and currency farming
   - Fast progression mechanics
   - Efficient task automation

#### 3. **Max Upgrades System**
   - Automatic character and ability upgrades
   - Progression optimization
   - Complete automation of upgrade chains

#### 4. **Keyless Execution**
   - Easy-to-use initialization
   - No key requirement for activation
   - Universal compatibility

### Frontend (UI)
- **HTML** (40.1%): Interface structure and layout
- **CSS** (50%): Styling, theming, and visual presentation

### Backend Logic
- **JavaScript** (9.9%): Core execution engine and feature management
- **Optimization Module**: Performance tuning and safe execution

## Key Features

✅ **Safe Progression** - Optimized to avoid detection  
✅ **Fast Execution** - Efficient script performance  
✅ **Complete Automation** - All abilities and upgrades automated  
✅ **Multi-Platform** - Works on Delta, mobile, and PC executors

## Workflow

1. User loads script via executor
2. Keyless execution initializes core modules
3. JavaScript engine manages feature logic
4. HTML/CSS provides user interface
5. Features execute simultaneously (Kill Aura, Auto Farm, Max Upgrades)
6. Optimization module ensures safe, fast operation

---

*Last Updated: 2026-01-29*