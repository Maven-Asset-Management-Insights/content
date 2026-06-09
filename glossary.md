---
layout: default
title: Glossary
permalink: /glossary/
categories:
  - glossary
search: true
---

<section class="hero">
  <h1>Glossary</h1>
  <p><strong>Clear definitions for Maximo, reliability, and asset performance concepts, grounded in outcomes.</strong></p>
</section>

<div class="glossary-shell">
  <div class="glossary-toolbar" role="search">
    <div class="glossary-search-wrap">
      <label class="sr-only" for="glossary-search">Search glossary</label>
      <input
        id="glossary-search"
        class="glossary-search"
        type="search"
        placeholder="Search terms or definitions"
        autocomplete="off"
      />
    </div>

    <div class="glossary-meta">
      <span id="glossary-count">0 terms</span>
      <button type="button" id="glossary-clear" class="glossary-clear">Clear</button>
    </div>
  </div>

 <div class="glossary-filters" id="glossary-filters" aria-label="Glossary category filters"></div>

  <nav id="top" class="glossary-nav" aria-label="Glossary index">
    <a href="#A">A</a>
    <a href="#B">B</a>
    <a href="#C">C</a>
    <a href="#D">D</a>
    <a href="#E">E</a>
    <a href="#F">F</a>
    <a href="#G">G</a>
    <a href="#H">H</a>
    <a href="#I">I</a>
    <a href="#J">J</a>
    <a href="#K">K</a>
    <a href="#L">L</a>
    <a href="#M">M</a>
    <a href="#N">N</a>
    <a href="#O">O</a>
    <a href="#P">P</a>
    <a href="#Q">Q</a>
    <a href="#R">R</a>
    <a href="#S">S</a>
    <a href="#T">T</a>
    <a href="#U">U</a>
    <a href="#V">V</a>
    <a href="#W">W</a>
    <a href="#X">X</a>
    <a href="#Y">Y</a>
    <a href="#Z">Z</a>
  </nav>

  <div id="glossary-empty" class="glossary-empty" hidden>
    No glossary terms match your search or selected category.
  </div>

  <div class="glossary" id="glossary-list">

    <h2 id="A">A</h2>

    <div class="glossary-term" data-category="maximo troubleshooting">
      <h3 id="appdoctype">APPDOCTYPE</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>APPDOCTYPE is a Maximo system table that defines document type configurations for applications, controlling how attachments and document references are associated with records like Work Orders, Assets, and Inspection Forms. When attachment behavior is inconsistent or documents fail to associate correctly, APPDOCTYPE configuration is often the place to investigate. Administrators modifying document handling in Maximo should understand which APPDOCTYPE entries apply to the affected application before making changes.</p>
    </div>

    <div class="glossary-term" data-category="licensing maximo">
      <h3 id="apppoints-licensing">AppPoints Licensing</h3>
      <div class="glossary-tags">
        <span>Licensing</span>
        <span>Maximo</span>
      </div>
      <p>AppPoints Licensing is the consumption-based licensing model used in the Maximo Application Suite (MAS), where shared capacity units — called AppPoints — are drawn down based on which applications a user accesses and at what level. Unlike traditional per-seat licensing, AppPoints allow organizations to allocate capacity flexibly across asset management, monitoring, and analytics capabilities without assigning fixed licenses to individual users. Understanding how AppPoints are consumed by different MAS applications is important when planning user access, managing licensing costs, and sizing a MAS environment. See also: Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="maximo maintenance">
      <h3 id="asset-maximo">Asset</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
      </div>
      <p>An Asset in Maximo is a physical piece of equipment with its own record, capturing location, parent-child relationships, maintenance history, and performance data across its operating life. Assets are the foundation of work management, reliability analysis, and lifecycle cost tracking in Maximo — everything from work orders to failure codes to condition readings ties back to an asset record. The quality and completeness of asset records directly affects the value of reporting and analysis. An incomplete or poorly structured asset registry limits what Maximo can tell you about your operations. See also: Asset Hierarchy, Asset Registry, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="reliability strategy">
      <h3 id="asset-criticality">Asset Criticality</h3>
      <div class="glossary-tags">
        <span>Reliability</span>
        <span>Strategy</span>
      </div>
      <p>Asset Criticality is a structured ranking of assets based on risk factors such as safety impact, production consequence, regulatory exposure, and cost of failure, used to prioritize where maintenance effort, reliability focus, and data quality investment matter most. Without criticality rankings, organizations default to treating all assets equally — which means critical equipment may not receive appropriate attention while resources are spent on assets where failure has minimal impact. Criticality is one of the first things to establish when building or improving a reliability strategy, and it directly informs maintenance task selection, PM frequency, and spare parts stocking decisions. See also: Reliability Strategy, Asset Performance Management (APM).</p>
    </div>

    <div class="glossary-term" data-category="analytics reliability">
      <h3 id="asset-health-index-ahi">Asset Health Index (AHI)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Asset Health Index is a composite score that represents the overall condition of an asset by combining performance data, failure history, condition monitoring readings, and other indicators into a single value. AHI gives operations and reliability teams a fast way to assess which assets need attention without reviewing individual data points across multiple systems. It is particularly useful in large fleets where manual review of every asset is impractical. The quality of an AHI depends entirely on the quality and consistency of the underlying data feeding it — a score built on incomplete or unreliable inputs can be misleading. See also: Condition Monitoring, Asset Performance, Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="maximo data-quality">
      <h3 id="asset-hierarchy">Asset Hierarchy</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
      </div>
      <p>Asset Hierarchy is the structured arrangement of assets into parent-child relationships in Maximo — typically organized by site, system, equipment, and component — enabling meaningful cost rollup, failure analysis, and performance reporting at every level. A well-built hierarchy makes it possible to answer questions like "what is the total maintenance cost for this production line?" or "which subsystem is driving the most failures?" A flat list of assets without hierarchy structure — an Asset Registry — cannot answer those questions. Many organizations build a registry and assume they have a hierarchy; the gap shows up when they try to analyze performance by system or justify capital investment. See also: Asset Registry, Hierarchy Integrity.</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="asset-lifecycle">Asset Lifecycle</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Asset Lifecycle is the managed journey of a physical asset from acquisition through commissioning, operation, maintenance, and disposal, including all decisions made along the way. Managing an asset lifecycle is a deliberate strategy — not just tracking how long an asset lasts. Lifecycle management includes decisions about maintenance approach, capital reinvestment, performance thresholds, and planned retirement. Organizations that treat lifecycle management as a strategic discipline — rather than a reactive process — make better capital decisions, reduce unplanned failures, and lower total cost of ownership over time. See also: Asset Lifespan, Asset Lifecycle Cost, Total Cost of Ownership (TCO).</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="asset-lifecycle-cost">Asset Lifecycle Cost</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Asset Lifecycle Cost is the total cost of owning and operating an asset from acquisition through disposal, encompassing capital expenditure, installation, operation, maintenance, downtime losses, and decommissioning. Lifecycle cost analysis gives organizations a complete picture of what an asset truly costs — not just what it costs to maintain. An asset that appears inexpensive on a maintenance budget may carry high lifecycle costs due to energy consumption, frequent downtime, or expensive end-of-life removal. Lifecycle cost is a key input to capital planning, asset replacement decisions, and investment justification. See also: Total Cost of Ownership (TCO), Maintenance Cost, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="strategy">
      <h3 id="asset-lifespan">Asset Lifespan</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Asset Lifespan is the total duration an asset operates from commissioning to retirement, measured in time, cycles, or usage. Lifespan describes how long an asset lasts; Asset Lifecycle describes how it is managed throughout that time. Organizations that focus only on lifespan — extending how long equipment runs — often miss the strategic decisions around maintenance approach, capital reinvestment, and decommissioning timing that define true lifecycle management. A long lifespan is not always the right goal if the cost of operating aging equipment exceeds the cost of replacement. See also: Asset Lifecycle, Asset Lifecycle Cost.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="asset-performance">Asset Performance</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Asset Performance is how effectively an asset delivers its intended function over time, measured across dimensions including availability, reliability, maintenance cost, and safety. High asset performance is not just a product of the equipment itself — it results from consistent maintenance execution, accurate data capture, appropriate reliability strategy, and disciplined work management. Organizations that track asset performance systematically can identify degradation early, justify investment, and make better decisions about when to repair versus replace. Poor data quality in Maximo is one of the most common barriers to meaningful asset performance analysis. See also: Asset Performance Management (APM), Reliability, Availability, Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="asset-performance-management-apm">Asset Performance Management (APM)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Asset Performance Management is a set of capabilities that connect asset condition, risk, and performance data to maintenance and investment decisions, helping organizations improve reliability and optimize how maintenance resources are deployed. APM is more narrowly focused than EAM — it concentrates on performance data, condition monitoring, and reliability analytics rather than the full scope of asset lifecycle management, procurement, and compliance that EAM covers. Vendors often use EAM and APM interchangeably when it suits them. They are not the same, and treating them as equivalent can lead to misaligned technology decisions. IBM Maximo includes APM capabilities within the broader MAS platform. See also: Enterprise Asset Management (EAM), Maximo Application Suite (MAS), Condition Monitoring.</p>
    </div>

    <div class="glossary-term" data-category="data-quality maximo">
      <h3 id="asset-registry">Asset Registry</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
      </div>
      <p>An Asset Registry is a list of assets an organization owns or manages, capturing basic identification information such as asset number, description, location, and classification. A registry is not the same as an Asset Hierarchy — a registry tells you what assets exist, while a hierarchy defines how they relate to each other as systems, subsystems, and components. Many organizations build a registry and assume they have a hierarchy; the gap shows up when they try to roll up costs, analyze failures by system, or report on performance at a plant or production line level. A complete, accurate registry is the necessary foundation for building a meaningful hierarchy. See also: Asset Hierarchy, Hierarchy Integrity.</p>
    </div>

    <div class="glossary-term" data-category="strategy">
      <h3 id="asset-acquisition">Asset Acquisition</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Asset Acquisition is the process of procuring, receiving, and putting into service a new physical asset — encompassing specification, vendor selection, procurement, delivery, installation, and handover to operations. How an asset is acquired has direct consequences for its entire operating life: poorly specified assets may not meet operational requirements, assets procured without spare parts strategies create inventory gaps, and assets handed over without proper documentation make commissioning and baseline establishment difficult. For plant managers, acquisition is one of the few points in an asset's life where lifecycle cost can be meaningfully influenced before it is locked in. See also: Commissioning, Asset Baseline, Spare Parts Strategy at Commissioning, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="strategy data-quality">
      <h3 id="asset-baseline">Asset Baseline</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Strategy</span>
      </div>
      <p>An Asset Baseline is the documented reference state of an asset at a defined point in time — typically at commissioning or after a major overhaul — capturing design specifications, installed configuration, performance parameters, and condition. The baseline establishes what "good" looks like for that asset, providing the foundation for measuring degradation, evaluating maintenance effectiveness, and making informed replacement decisions later in the asset's life. In Maximo, asset baseline data is captured through asset records, specifications, and measurement points. Organizations that skip baseline documentation at commissioning often find themselves unable to answer basic questions about asset condition years later. See also: Asset Acquisition, Commissioning, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="asset-replacement-value-arv">Asset Replacement Value (ARV)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Asset Replacement Value (ARV) is the estimated cost to replace an asset with a new equivalent at current prices, used as a benchmark for evaluating maintenance investment, insurance coverage, and capital planning decisions. ARV provides critical context for maintenance budget discussions: maintenance spend expressed as a percentage of ARV is a widely used industry benchmark for assessing whether an asset is being appropriately maintained or under-invested. For plant managers and reliability professionals, ARV helps frame conversations with finance and leadership about whether the maintenance budget is adequate relative to the value of the assets it is protecting. See also: Total Cost of Ownership (TCO), Capital Expenditure (CapEx), Maintenance Backlog Ratio.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="asset-utilization">Asset Utilization</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Asset Utilization is the proportion of available time or capacity that an asset is actively being used for its intended productive purpose, expressed as actual output divided by maximum possible output over a defined period. Utilization is distinct from Availability — an asset can be available (ready to operate) but not utilized (not needed or not running). For operations and plant managers, utilization data informs decisions about asset rationalization, capacity planning, and whether investment in reliability improvement will actually translate to business value. A highly reliable asset with very low utilization may not justify significant reliability investment; a heavily utilized asset with poor reliability has an outsized impact on operations. See also: Availability, Asset Performance, Reliability.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="availability">Availability</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Availability is the proportion of time an asset is in a condition to perform its required function, expressed as uptime divided by total time including both scheduled and unscheduled downtime. Availability is often confused with Reliability, but they measure different things: Reliability is the probability an asset will not fail during a defined operating period, while Availability factors in all time the asset is out of service — including planned maintenance. An asset can be highly reliable (rarely fails unexpectedly) but have low availability if it is frequently taken offline for scheduled PMs. Treating Availability and Reliability as the same number in KPI reporting leads to poor decisions about maintenance strategy and capital investment. See also: Reliability, Operational Availability (Ao), Mean Time Between Failures (MTBF).</p>
    </div>


    <h2 id="B">B</h2>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="backlog-health">Backlog Health</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Backlog Health is a measure of how manageable, current, and well-prioritized the open maintenance work queue is, helping organizations ensure that critical reliability tasks can be planned and completed without excessive delay. A healthy backlog is not an empty one — some level of approved, queued work is normal and expected. An unhealthy backlog is one where work is aging unaddressed, priority is unclear, critical tasks are buried alongside low-value requests, or the volume has grown beyond the team's capacity to execute. Backlog Health is distinct from Deferred Maintenance: the backlog includes all open approved work, while deferred maintenance is specifically work that has been pushed past its due date. Tracking both separately is important for accurate risk assessment. See also: Deferred Maintenance, Planned vs. Unplanned Work, Maintenance Backlog Ratio.</p>
    </div>

    <div class="glossary-term" data-category="analytics maintenance strategy">
      <h3 id="maintenance-backlog-ratio">Maintenance Backlog Ratio</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Maintenance Backlog Ratio is a financial metric that expresses the total estimated cost of deferred or outstanding maintenance as a percentage of Asset Replacement Value (ARV), used to assess whether a facility or asset portfolio is being adequately maintained relative to its capital value. An industry rule of thumb holds that a backlog ratio above 2–5% of ARV represents meaningful deferred risk; ratios significantly higher indicate chronic under-investment. For plant managers, the backlog ratio is one of the most effective tools for communicating maintenance funding needs to finance and leadership in terms they understand — not work order counts, but capital exposure. See also: Asset Replacement Value (ARV), Deferred Maintenance, Backlog Health.</p>
    </div>


    <h2 id="C">C</h2>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="capital-expenditure-capex">Capital Expenditure (CapEx)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Capital Expenditure (CapEx) is spending used to acquire, upgrade, or extend the life of a physical asset — recorded on the balance sheet and depreciated over time rather than expensed immediately. In asset management, CapEx typically funds new asset acquisition, major overhauls, life extension projects, and replacement of end-of-life equipment. Understanding the distinction between CapEx and OpEx matters because the two are funded from different budgets, approved through different processes, and carry different financial implications. For plant managers and reliability professionals, the ability to justify CapEx requests with lifecycle cost data, asset condition evidence, and failure history from Maximo is one of the most valuable outcomes of a well-governed EAM program. See also: Operating Expenditure (OpEx), Capital Plan, Asset Replacement Value (ARV), Total Cost of Ownership (TCO).</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="capital-plan">Capital Plan</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>A Capital Plan is a multi-year forecast of planned capital expenditures for asset replacement, life extension, and new capacity — aligned to operational priorities, asset condition data, and available funding. Capital plans translate asset lifecycle strategy into financial commitments, helping organizations avoid the reactive scramble of replacing assets only after they fail catastrophically. For plant managers, a credible capital plan is built on asset health data, remaining useful life estimates, and failure history — the kind of evidence that Maximo, when well-maintained, is designed to provide. Organizations without disciplined asset data often find their capital plans are based on age and intuition rather than condition and risk. See also: Capital Expenditure (CapEx), Asset Replacement Value (ARV), Remaining Useful Life (RUL), Lifecycle Replacement Decision.</p>
    </div>

    <div class="glossary-term" data-category="strategy">
      <h3 id="commissioning">Commissioning</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Commissioning is the structured process of verifying, testing, and formally accepting a new or significantly modified asset into operational service — confirming that it performs to specification before responsibility transfers from the project or installation team to operations and maintenance. Commissioning is a critical lifecycle transition point: assets commissioned without proper documentation, baseline data capture, or PM setup in Maximo start their operating life with structural gaps that are difficult and expensive to close later. For plant managers and reliability professionals, commissioning is the opportunity to establish the asset record, load the baseline, create the initial PM program, and ensure spare parts are stocked before the first failure occurs. See also: Pre-Commissioning, Asset Baseline, Asset Acquisition, Spare Parts Strategy at Commissioning.</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy">
      <h3 id="cmms">Computerized Maintenance Management System (CMMS)</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>A Computerized Maintenance Management System (CMMS) is software designed to manage maintenance operations — work orders, preventive maintenance schedules, technician assignments, and spare parts inventory — helping keep equipment running day to day. A CMMS focuses on maintenance execution. Enterprise Asset Management (EAM) expands beyond maintenance to cover the full asset lifecycle, connecting maintenance execution with capital planning, compliance, and strategic decisions. The short version: a CMMS can function within an EAM, but an EAM is not just a CMMS. IBM Maximo is an EAM platform that includes CMMS capabilities and much more. See also: Enterprise Asset Management (EAM), Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="data-quality maintenance">
      <h3 id="closeout-quality">Closeout Quality</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maintenance</span>
      </div>
      <p>Closeout Quality is the consistency and completeness of data captured when work orders are finished, including failure codes, actual labor and materials, work performed descriptions, and any follow-up actions identified. Closeout data is the primary source of maintenance history in Maximo — it feeds failure analysis, reliability reporting, PM optimization, and cost tracking. When closeout quality is poor, those downstream analyses produce unreliable results regardless of how sophisticated the tools are. Common causes of poor closeout quality include unclear expectations, mobile usability friction, and lack of accountability in the work completion process. See also: Work Order Closeout, Work Order Data Quality, Failure Code.</p>
    </div>

    <div class="glossary-term" data-category="analytics reliability integration">
      <h3 id="condition-monitoring">Condition Monitoring</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Integration</span>
        <span>Reliability</span>
      </div>
      <p>Condition Monitoring is the ongoing tracking of asset health indicators — such as vibration, temperature, pressure, current draw, or oil analysis — to detect changes that may indicate developing faults before failure occurs. Condition monitoring data can be collected manually during inspections, through fixed sensors, or through IoT-connected devices integrated with Maximo. When integrated effectively, condition data supports Condition-Based Maintenance (CBM) and Predictive Maintenance (PdM) strategies, allowing teams to act on what the equipment is telling them rather than following fixed schedules. The value of condition monitoring is realized only when the data is acted upon consistently. See also: Condition-Based Maintenance (CBM), Predictive Maintenance (PdM), Internet of Things (IoT).</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="condition-based-maintenance-cbm">Condition-Based Maintenance (CBM)</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Condition-Based Maintenance is a maintenance strategy where work is performed based on the actual condition of an asset rather than on fixed time intervals, helping reduce unnecessary maintenance and prevent failures before they affect operations. CBM relies on condition monitoring data — such as vibration readings, temperature trends, or oil analysis — to trigger maintenance when a defined threshold is crossed. It is related to but distinct from Predictive Maintenance (PdM): CBM reacts when a condition indicator crosses a threshold, while PdM uses data models to forecast when that threshold will be crossed before it happens. Both strategies are more effective than fixed-interval PM for appropriate asset classes. See also: Predictive Maintenance (PdM), Condition Monitoring, Preventive Maintenance (PM).</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="corrective-maintenance-cm">Corrective Maintenance (CM)</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Corrective Maintenance is work performed to restore an asset after a fault has been identified, returning it to normal operation and preventing further degradation. Corrective Maintenance is often confused with Reactive Maintenance, but they are not the same. Planned corrective maintenance — identifying a developing fault and scheduling its repair before failure occurs — is a legitimate and intentional strategy. Reactive maintenance is the unplanned version: discovering a failure after it has already disrupted operations. An organization with a mature reliability strategy will have a defined place for planned corrective work; the goal is to minimize unplanned reactive work, not to eliminate corrective maintenance entirely. See also: Reactive Work, Reliability Strategy.</p>
    </div>


    <h2 id="D">D</h2>

    <div class="glossary-term" data-category="data-quality analytics">
      <h3 id="data-confidence">Data Confidence</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Data Quality</span>
      </div>
      <p>Data Confidence is the level of trust that operations, reliability, and management teams have in the accuracy and consistency of data in Maximo, enabling decisions to be based on what the system says rather than on workarounds, manual spreadsheets, or institutional knowledge. Low data confidence is one of the most common and costly consequences of poor data governance — teams stop relying on the system, reporting becomes unreliable, and the value of Maximo investment erodes. Building data confidence requires consistent standards, clear accountability, and sustained attention to data quality over time. It is earned gradually and lost quickly. See also: Data Quality, Data Governance, Data Discipline.</p>
    </div>

    <div class="glossary-term" data-category="data-quality">
      <h3 id="data-consistency">Data Consistency</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
      </div>
      <p>Data Consistency is the uniformity of how information is entered, classified, and maintained across systems, teams, and time in Maximo, ensuring that data can be compared, aggregated, and analyzed reliably. Inconsistent data — the same asset described differently by different crews, failure codes applied with different meanings, work types used interchangeably — produces reporting that looks complete but cannot be trusted. Data consistency is not achieved through a one-time cleanup; it requires ongoing standards, training, and enforcement. See also: Data Governance, Data Standard Enforcement, Data Discipline.</p>
    </div>

    <div class="glossary-term" data-category="data-quality governance">
      <h3 id="data-discipline">Data Discipline</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
      </div>
      <p>Data Discipline is the consistent application of standards and practices for entering and maintaining data in Maximo, day after day and across all users and teams. Data Discipline is what separates a one-time data cleanup from sustained data quality. Without it, even well-structured data degrades over time as entry habits drift and standards are applied inconsistently. Building data discipline requires clear expectations, embedded standards in workflows, leadership reinforcement, and accountability for data quality as part of the work management process. See also: Data Governance, Data Standard Enforcement, Data Drift.</p>
    </div>

    <div class="glossary-term" data-category="data-quality governance">
      <h3 id="data-drift">Data Drift</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
      </div>
      <p>Data Drift is the gradual degradation of data quality over time that occurs when standards are inconsistently applied, oversight lapses, or new users are not properly trained. Unlike a sudden data quality failure, drift is slow and often invisible until it has significantly undermined reporting and decision-making. Organizations that complete a Maximo data cleanup but do not address the underlying practices that caused the problem will experience drift again — usually within months. Preventing data drift requires ongoing governance, not just periodic remediation. See also: Data Discipline, Data Governance, Data Confidence.</p>
    </div>

    <div class="glossary-term" data-category="data-quality governance strategy">
      <h3 id="data-governance">Data Governance</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
        <span>Strategy</span>
      </div>
      <p>Data Governance is the organizational structure of standards, ownership, roles, and processes used to maintain accurate, consistent, and trustworthy data in Maximo over time. Effective data governance defines who is responsible for data quality in each domain, what the standards are, how compliance is monitored, and how issues are resolved. Without governance, data quality depends on individual habits rather than organizational standards — and individual habits vary. Data governance is not an IT function alone; it requires active participation from operations, reliability, and management to be effective. See also: Data Quality, Data Discipline, Master Data Management (MDM).</p>
    </div>

    <div class="glossary-term" data-category="analytics data-quality governance">
      <h3 id="data-lineage">Data Lineage</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Data Quality</span>
        <span>Governance</span>
      </div>
      <p>Data Lineage tracks the origin of data, the transformations it undergoes, and where it is used across systems and reports, helping ensure transparency and accountability in data-driven decisions. In a Maximo context, data lineage matters when trying to understand why a report shows a particular result, where a calculation comes from, or how an integration is passing data between systems. When data lineage is unclear, investigating anomalies becomes time-consuming and root causes are difficult to establish. See also: Data Governance, Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="data-quality maximo">
      <h3 id="data-quality">Data Quality</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
      </div>
      <p>Data Quality is the completeness, consistency, and accuracy of data in Maximo — including asset records, work order history, failure codes, labor entries, and inventory transactions — that determines how much the system can actually be trusted to support decisions. High data quality means the system reflects reality. Low data quality means reports are unreliable, failure analysis is guesswork, and the investment in Maximo does not deliver its full value. Data quality is not a technology problem — it is a people, process, and standards problem that technology can support but not solve on its own. See also: Data Governance, Data Discipline, Data Confidence, Work Order Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="data-quality governance">
      <h3 id="data-standard-enforcement">Data Standard Enforcement</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
      </div>
      <p>Data Standard Enforcement is the active monitoring and correction of data entry to ensure that defined naming conventions, classification codes, and input rules are consistently followed in Maximo. Standards without enforcement produce the same result as having no standards — they are followed selectively and degrade over time. Enforcement can be built into the system through required fields, validated picklists, and workflow controls, and reinforced through supervisory review and regular data quality audits. See also: Data Governance, Data Discipline, Data Consistency.</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="deferred-maintenance">Deferred Maintenance</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Deferred Maintenance is work that has been identified and approved but intentionally postponed past its due date, creating known and documented risk. Deferred maintenance is not the same as backlog. A backlog includes all open, approved work waiting to be scheduled — including work that is current and on track. Deferred maintenance is the subset that has been pushed past when it should have been done. Treating all backlog as deferred distorts the risk picture and makes it harder to prioritize capital requests or justify maintenance investment. Tracking deferred maintenance separately and explicitly — with clear accountability and risk documentation — is a sign of a mature maintenance organization. See also: Backlog Health, Maintenance Backlog Ratio, Planned vs. Unplanned Work.</p>
    </div>

    <div class="glossary-term" data-category="strategy">
      <h3 id="decommissioning">Decommissioning</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Decommissioning is the planned process of safely retiring an asset from active service — including isolation, removal, remediation of any environmental hazards, and final disposition of the physical equipment. Decommissioning is the final stage of the asset lifecycle and, like commissioning, is more expensive and disruptive when not planned in advance. For plant managers, decommissioning decisions should be driven by lifecycle cost analysis, remaining useful life estimates, and operational strategy — not just by failure or crisis. In Maximo, decommissioned assets should be formally retired in the system to preserve their history while removing them from active maintenance schedules and inventory planning. See also: Asset Disposal, Asset Write-Off, Asset Lifecycle, Lifecycle Replacement Decision.</p>
    </div>

    <div class="glossary-term" data-category="strategy">
      <h3 id="asset-disposal">Asset Disposal</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Asset Disposal is the process of removing a decommissioned asset from inventory and operational records through sale, transfer, salvage, scrapping, or regulated disposal — including any financial, environmental, and documentation requirements associated with the method chosen. Disposal is not simply the physical removal of equipment; it has accounting, regulatory, and data management dimensions. In Maximo, proper disposal requires retiring the asset record, closing out any open work orders, and capturing final condition and cost data before the record is archived. Incomplete disposal processes leave ghost assets in the system — records that appear active but represent equipment that no longer exists — which distorts asset counts, maintenance plans, and reporting. See also: Decommissioning, Asset Write-Off, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="analytics integration maximo">
      <h3 id="digital-twin">Digital Twin</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Integration</span>
        <span>Maximo</span>
      </div>
      <p>A Digital Twin is a virtual representation of a physical asset that is continuously updated with real-time operational data, enabling teams to monitor condition, simulate scenarios, and anticipate performance changes without physical inspection. In the context of Maximo and IBM MAS, digital twin capabilities connect sensor data, condition monitoring feeds, and maintenance history to create a live model of asset behavior. The value of a digital twin depends on the quality and completeness of both the real-time data feeding it and the historical maintenance data behind it. See also: Condition Monitoring, Internet of Things (IoT), Maximo Application Suite (MAS).</p>
    </div>


    <h2 id="E">E</h2>

    <div class="glossary-term" data-category="strategy maximo">
      <h3 id="enterprise-asset-management-eam">Enterprise Asset Management (EAM)</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Strategy</span>
      </div>
      <p>Enterprise Asset Management is a structured approach to managing physical assets across their full lifecycle — from acquisition and commissioning through operation, maintenance, and disposal — helping organizations optimize performance, control cost, and manage risk. EAM is broader in scope than a CMMS, which focuses primarily on day-to-day maintenance operations. EAM connects maintenance execution with capital planning, regulatory compliance, reliability strategy, and financial decision-making. IBM Maximo is an EAM platform. Organizations that treat Maximo only as a work order system are using a small fraction of what EAM is designed to deliver. See also: Computerized Maintenance Management System (CMMS), Asset Performance Management (APM), Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="strategy maximo">
      <h3 id="eam-strategy">Enterprise Asset Management (EAM) Strategy</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Strategy</span>
      </div>
      <p>EAM Strategy is the organizational plan that defines how asset management practices align with business goals, guiding decisions about maintenance approaches, reliability investment, technology, data governance, and capital planning. A well-defined EAM strategy ensures that Maximo is configured and used in a way that supports operational objectives — not just as a system of record, but as a system of discipline. Organizations without a clear EAM strategy often find their Maximo implementations drifting over time, with data quality degrading and the system failing to deliver the visibility leadership expects. See also: Enterprise Asset Management (EAM), Reliability Strategy.</p>
    </div>

    <div class="glossary-term" data-category="reliability strategy">
      <h3 id="end-of-life-eol">End-of-Life (EOL)</h3>
      <div class="glossary-tags">
        <span>Reliability</span>
        <span>Strategy</span>
      </div>
      <p>End-of-Life (EOL) is the point in an asset's lifecycle at which it is no longer economical or practical to continue operating and maintaining it — due to deteriorating condition, prohibitive maintenance costs, obsolescence, regulatory requirements, or inability to meet performance standards. EOL is not simply a function of age; an asset can reach end-of-life early due to severe duty cycles or poor maintenance, or exceed its design life through excellent care and operating conditions. For reliability professionals, identifying EOL proactively — using condition data, remaining useful life estimates, and lifecycle cost analysis — is far preferable to discovering it reactively after a catastrophic failure. For plant managers, EOL assets that remain in service without a replacement plan represent accumulating risk. See also: Remaining Useful Life (RUL), Lifecycle Replacement Decision, Decommissioning, Asset Lifecycle Cost.</p>
    </div>

    <div class="glossary-term" data-category="data-quality maintenance">
      <h3 id="execution-alignment">Execution Alignment</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maintenance</span>
      </div>
      <p>Execution Alignment is the degree to which what actually happens in the field matches what was planned and recorded in Maximo — including scope, labor, materials, and timing. When execution alignment is high, Maximo data reflects reality and can be trusted for analysis, reporting, and planning. When it is low, the system shows one picture while the field operates differently, producing unreliable history and undermining the value of the entire work management process. Execution alignment problems are often symptoms of poor planning, inadequate training, mobile usability issues, or a culture where Maximo is seen as a reporting burden rather than a work management tool. See also: Work Order Data Quality, Planning Accuracy, Work Management Discipline.</p>
    </div>


    <h2 id="F">F</h2>

    <div class="glossary-term" data-category="reliability data-quality">
      <h3 id="failure-code">Failure Code</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Reliability</span>
      </div>
      <p>A Failure Code is a standardized classification applied to a work order during closeout that records what failed, where it failed, and why — typically using a structured Problem-Cause-Remedy or similar coding framework in Maximo. Failure codes are the primary input to failure analysis, recurring failure identification, and reliability improvement. When failure codes are missing, generic, or applied inconsistently, the maintenance history in Maximo cannot support meaningful analysis — and organizations are left reacting to failures they could have anticipated. A well-designed failure code taxonomy, consistently applied, is one of the highest-value data quality investments a maintenance organization can make. See also: Standardized Failure Codes, Failure Data Quality, Root Cause Analysis (RCA).</p>
    </div>

    <div class="glossary-term" data-category="data-quality reliability">
      <h3 id="failure-data-quality">Failure Data Quality</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Reliability</span>
      </div>
      <p>Failure Data Quality is the accuracy and completeness of failure-related information captured in Maximo work orders, including failure codes, problem descriptions, cause classifications, and corrective actions taken. High failure data quality makes it possible to identify recurring failure patterns, perform root cause analysis, and optimize maintenance strategies based on actual history. Low failure data quality — generic codes, missing fields, or inconsistent application — produces history that looks complete but cannot support analysis. Improving failure data quality requires both technical structure (a good taxonomy) and behavioral change (consistent application by the people closing work orders). See also: Failure Code, Closeout Quality, Root Cause Analysis (RCA).</p>
    </div>

    <div class="glossary-term" data-category="reliability">
      <h3 id="failure-mode">Failure Mode</h3>
      <div class="glossary-tags">
        <span>Reliability</span>
      </div>
      <p>A Failure Mode is the specific mechanism by which an asset fails to perform its required function — not just that it failed, but how and why. Understanding failure modes is foundational to reliability engineering: it allows teams to design maintenance strategies that address the actual causes of failure rather than simply reacting after the fact. When failure modes are documented and coded consistently in Maximo, patterns emerge — which assets fail the same way repeatedly, where PM strategies have gaps, and where maintenance spend is leaking into preventable failures. Without failure mode data, maintenance history is just a list of dates and costs. See also: Failure Code, Failure Modes Effects and Criticality Analysis (FMECA), Root Cause Analysis (RCA).</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="fmeca">Failure Modes, Effects, and Criticality Analysis (FMECA)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>FMECA is a structured reliability engineering method for systematically identifying the ways an asset or system can fail, evaluating the consequences of each failure mode, and prioritizing actions based on the combined risk of likelihood and impact. FMECA goes beyond identifying what can go wrong — it quantifies criticality, helping reliability teams focus attention and resources where failure risk is highest. FMECA outputs directly inform maintenance task selection, inspection frequencies, and spare parts strategies. It is most valuable for critical assets where unplanned failure has significant safety, production, or cost consequences. See also: Failure Mode, Asset Criticality, Reliability Strategy.</p>
    </div>


    <h2 id="H">H</h2>

    <div class="glossary-term" data-category="data-quality maximo">
      <h3 id="hierarchy-integrity">Hierarchy Integrity</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
      </div>
      <p>Hierarchy Integrity is the accuracy and completeness of parent-child relationships within the asset hierarchy in Maximo, ensuring that assets are correctly associated with their systems, subsystems, and locations so that cost rollup, failure analysis, and performance reporting reflect the true operational structure. Poor hierarchy integrity — missing parent relationships, incorrectly assigned assets, or flat registries mistaken for hierarchies — produces reporting that cannot be trusted at the system or plant level. Hierarchy integrity issues are common after migrations, upgrades, or periods of rapid asset additions without governance oversight. See also: Asset Hierarchy, Asset Registry, Data Governance.</p>
    </div>


    <h2 id="I">I</h2>

    <div class="glossary-term" data-category="maximo strategy licensing">
      <h3 id="ibm-control-desk">IBM Control Desk</h3>
      <div class="glossary-tags">
        <span>Licensing</span>
        <span>Maximo</span>
        <span>Strategy</span>
      </div>
      <p>IBM Control Desk was an IBM platform that combined IT service management (ITSM) and IT asset management (ITAM) capabilities, historically deployed alongside Maximo in organizations that needed to manage both physical and IT assets. Related capabilities have since shifted into newer IBM suites, and organizations on Control Desk should evaluate their current roadmap in the context of IBM's current portfolio. See also: IT Service Management (ITSM), Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="maximo troubleshooting mobile">
      <h3 id="inspection-form">Inspection Form</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Mobile</span>
        <span>Troubleshooting</span>
      </div>
      <p>An Inspection Form in Maximo is a structured record used to capture field inspection data through a defined set of questions and response types, helping standardize how technicians assess and document asset condition during inspections. Inspection Forms support consistent condition assessments across different crews and shifts, feeding condition monitoring programs and maintenance decision-making. In Maximo Mobile, Inspection Forms are completed directly on a technician's device. Configuration of Inspection Forms involves APPDOCTYPE settings, and revisions to existing forms require care to preserve prior response history. See also: Inspection Form Revision, APPDOCTYPE, Mobile Object Structures.</p>
    </div>

    <div class="glossary-term" data-category="maximo troubleshooting">
      <h3 id="inspection-form-revision">Inspection Form Revision</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>Inspection Form Revision is the process of creating an updated version of an existing Inspection Form in Maximo when inspection criteria need to change, while preserving the response history tied to previous versions. Revising an Inspection Form incorrectly — editing in place rather than creating a new revision — can corrupt or orphan historical response data, making past inspection records inaccessible or unreliable. Understanding Maximo's revision workflow is essential before modifying any Inspection Form that has been used in the field. See also: Inspection Form, APPDOCTYPE.</p>
    </div>

    <div class="glossary-term" data-category="analytics integration maximo">
      <h3 id="internet-of-things-iot">Internet of Things (IoT)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Integration</span>
        <span>Maximo</span>
      </div>
      <p>The Internet of Things (IoT) refers to a network of connected sensors, devices, and equipment that continuously collect and transmit real-time operational data — such as temperature, vibration, pressure, and runtime — to systems like Maximo for analysis and action. IoT integration enables condition-based and predictive maintenance strategies by feeding live asset health data directly into the work management and analytics environment. IBM MAS includes IoT monitoring capabilities through Maximo Monitor, allowing organizations to set alert thresholds, trigger work orders automatically, and track asset condition over time. The value of IoT data depends on the quality of the integration and the reliability of the sensor data feeding it. See also: Condition Monitoring, Predictive Maintenance (PdM), Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy">
      <h3 id="inventory-optimization">Inventory Optimization</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Inventory Optimization is the process of balancing spare parts availability against carrying cost, ensuring that critical materials are on hand when needed without overstocking items that tie up capital and warehouse space. In Maximo, inventory optimization involves analyzing stocking levels against historical consumption, lead times, asset criticality, and failure risk. Under-stocking critical spares extends downtime when failures occur; over-stocking drains capital on parts that may never be used. Inventory decisions should be driven by asset criticality and maintenance strategy, not by historical habits or fear of stockouts alone. See also: Asset Criticality, Reliability Strategy.</p>
    </div>

    <div class="glossary-term" data-category="strategy integration">
      <h3 id="it-service-management">IT Service Management (ITSM)</h3>
      <div class="glossary-tags">
        <span>Integration</span>
        <span>Strategy</span>
      </div>
      <p>IT Service Management (ITSM) is a structured approach to planning, delivering, and improving IT services through defined processes and workflows, covering incident management, change control, service requests, and problem resolution. ITSM and EAM are distinct disciplines — ITSM manages IT services and assets, while EAM manages physical operational assets — but they increasingly intersect as organizations manage both physical and digital infrastructure in shared environments. IBM Maximo for IT extends Maximo's capabilities into ITSM use cases, and integrations between Maximo and ITSM platforms are common in complex asset-intensive organizations. See also: Enterprise Asset Management (EAM), IBM Control Desk.</p>
    </div>


    <h2 id="J">J</h2>

    <div class="glossary-term" data-category="maximo maintenance mobile">
      <h3 id="job-plan">Job Plan</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
        <span>Mobile</span>
      </div>
      <p>A Job Plan in Maximo is a reusable template that defines the steps, estimated labor, required materials, and tools needed to complete a specific maintenance task. When applied to a work order, the Job Plan pre-populates the work order with everything the planner and technician need, improving planning accuracy, reducing variability in execution, and producing consistent, comparable closeout data. Job Plans are one of the most powerful and most underused features in Maximo. When they are missing or incomplete, planners rebuild the same information repeatedly, technicians work from memory rather than procedure, and the resulting work order data is too inconsistent to support meaningful analysis. Well-maintained Job Plans are the foundation of disciplined work management. See also: Standard Job Plan, Planning Accuracy, Work Order Data Quality.</p>
    </div>


    <h2 id="K">K</h2>

    <div class="glossary-term" data-category="analytics strategy governance">
      <h3 id="kpi">Key Performance Indicator (KPI)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Governance</span>
        <span>Strategy</span>
      </div>
      <p>A Key Performance Indicator (KPI) is a quantifiable metric used to measure progress toward a defined operational or strategic goal, helping teams track outcomes such as PM compliance, backlog levels, planned-to-unplanned work ratios, or mean time between failures. In asset management, KPIs are only as reliable as the data feeding them — a PM compliance KPI built on incomplete work order closeouts will misrepresent actual performance. Selecting the right KPIs, defining them precisely, and ensuring the underlying data is trustworthy are all prerequisites for KPIs to drive the right behaviors and decisions. See also: Key Risk Indicator (KRI), Data Quality, PM Compliance.</p>
    </div>

    <div class="glossary-term" data-category="analytics strategy">
      <h3 id="key-risk-indicator-kri">Key Risk Indicator (KRI)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>A Key Risk Indicator (KRI) is a metric that signals increasing operational or asset risk — providing an early warning that conditions are deteriorating before performance is visibly affected. While KPIs measure current performance, KRIs look ahead at exposure. In asset management, KRIs might track the rate of deferred maintenance growth, the percentage of critical assets without updated inspection records, or rising reactive work ratios. Monitoring KRIs alongside KPIs gives leadership a more complete picture of both current performance and emerging risk. See also: Key Performance Indicator (KPI), Asset Criticality, Deferred Maintenance.</p>
    </div>


    <h2 id="M">M</h2>

    <div class="glossary-term" data-category="data-quality governance strategy">
      <h3 id="master-data-management-mdm">Master Data Management (MDM)</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
        <span>Strategy</span>
      </div>
      <p>Master Data Management (MDM) is a governance discipline that establishes and maintains a single, authoritative, and consistent set of core data records — such as assets, locations, materials, and vendors — across systems and over time. In a Maximo context, MDM governs how foundational records are created, classified, and maintained to ensure that data is reliable and comparable across the organization. Without MDM, the same asset may exist under different names in different systems, materials may be duplicated under multiple part numbers, and reporting across locations becomes unreliable. MDM is especially important in multi-site organizations and during system integrations or migrations. See also: Data Governance, Data Quality, Asset Registry.</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy analytics">
      <h3 id="maintenance-cost">Maintenance Cost</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Maintenance Cost is the total expenditure associated with maintaining an asset, including planned and unplanned labor, materials, contractor costs, and associated overhead. Maintenance Cost is one component of Total Cost of Ownership (TCO), but not the whole picture. An asset that is inexpensive to maintain may still carry poor TCO if it is costly to operate, energy-intensive, or expensive to decommission. Organizations that optimize only for maintenance spend often miss the larger investment picture. Tracking maintenance cost accurately in Maximo — through proper work order costing, labor entry, and material transactions — is a prerequisite for meaningful lifecycle cost analysis. See also: Total Cost of Ownership (TCO), Asset Lifecycle Cost, Maintenance Backlog Ratio.</p>
    </div>

    <div class="glossary-term" data-category="licensing maximo strategy">
      <h3 id="maximo-application-suite">Maximo Application Suite (MAS)</h3>
      <div class="glossary-tags">
        <span>Licensing</span>
        <span>Maximo</span>
        <span>Strategy</span>
      </div>
      <p>Maximo Application Suite (MAS) is IBM's modern platform for enterprise asset management and operational intelligence, bringing together core Maximo EAM capabilities with Maximo Monitor (IoT and condition monitoring), Maximo Predict (AI-driven predictive maintenance), Maximo Visual Inspection (computer vision for inspections), and Maximo Health (asset health scoring) under a single licensing and deployment model. MAS represents IBM's strategic direction for Maximo, and organizations on older Maximo versions should understand the MAS roadmap and what a migration involves before planning their next upgrade. Licensing in MAS is based on AppPoints rather than traditional per-seat models. See also: AppPoints Licensing, Enterprise Asset Management (EAM), Predictive Maintenance (PdM).</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="mtbf">Mean Time Between Failures (MTBF)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Mean Time Between Failures (MTBF) is the average operating time between consecutive failures of a repairable asset, used as a primary metric for evaluating asset reliability and comparing performance over time or across similar equipment. A rising MTBF indicates improving reliability; a declining MTBF is an early warning of degradation. MTBF is only meaningful when failure events are captured consistently and completely in Maximo — gaps in failure recording distort the calculation and can mask real reliability trends. MTBF should be interpreted alongside MTTR to understand both how often an asset fails and how quickly it is restored. See also: Mean Time To Repair (MTTR), Reliability, Failure Code.</p>
    </div>

    <div class="glossary-term" data-category="maximo mobile">
      <h3 id="mobile-object-structures">Mobile Object Structures</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Mobile</span>
      </div>
      <p>Mobile Object Structures are the OSLC-based data structures that define which Maximo records, fields, and relationships are synchronized to a technician's device for use in Maximo Mobile. Because the mobile application queries a local on-device database rather than Maximo directly, only data included in the relevant Mobile Object Structures is available offline. Fields or relationships not defined in these structures will not appear in the mobile application, even when they are accessible in the browser-based application (RBA). Understanding Mobile Object Structures is essential when troubleshooting missing fields in Maximo Mobile or customizing the mobile experience. See also: Inspection Form, Residual State.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="mttr">Mean Time To Repair (MTTR)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Mean Time To Repair (MTTR) is the average time required to restore an asset to normal operation after a failure, measuring the efficiency and effectiveness of the maintenance response. A lower MTTR reflects faster diagnosis, better parts availability, clearer repair procedures, and more effective technician support. MTTR is most meaningful when paired with MTBF — an asset that fails frequently but is restored quickly has a different operational profile than one that fails rarely but takes a long time to repair. Accurate MTTR calculation depends on consistent capture of failure start and end times in Maximo work orders. See also: Mean Time Between Failures (MTBF), Reliability, Availability.</p>
    </div>

    <div class="glossary-term" data-category="maximo troubleshooting">
      <h3 id="mid-transaction-failure">Mid-Transaction Failure</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>A Mid-Transaction Failure occurs when a Maximo operation — such as a save, status change, or record update — fails partway through execution, leaving the system in an inconsistent state where some fields or flags reflect the attempted action while others reflect the prior state. Mid-transaction failures can cause unexpected behavior in Maximo applications, including records that appear locked, status fields that cannot be updated, or workflows that fail to advance. Resolving them typically requires identifying and correcting the residual state left by the incomplete operation rather than simply retrying the transaction. See also: Residual State, Transaction Rollback, System Record Integrity.</p>
    </div>


    <h2 id="O">O</h2>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="operating-expenditure-opex">Operating Expenditure (OpEx)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Operating Expenditure (OpEx) is day-to-day spending required to run and maintain operations — expensed in the period incurred rather than capitalized and depreciated over time. In asset management, OpEx covers routine maintenance labor, spare parts consumption, contractor services, and other recurring costs of keeping assets operational. The CapEx versus OpEx distinction matters practically for plant managers and reliability professionals because the two are funded, approved, and reported differently. A major overhaul that extends asset life beyond its original design may qualify as CapEx; routine maintenance does not. Understanding how maintenance activities are classified affects budget planning, financial reporting, and the ability to justify investment. See also: Capital Expenditure (CapEx), Maintenance Cost, Total Cost of Ownership (TCO).</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="operational-availability-ao">Operational Availability (Ao)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Operational Availability (Ao) is the probability that an asset is in an operable and committable state at a random point in time, accounting for all sources of downtime including scheduled maintenance, unplanned failures, and logistical delays such as waiting for parts or personnel. Ao is a more complete availability measure than simple uptime percentage because it reflects the real-world factors that prevent an asset from being used when needed. It is particularly relevant for critical assets in military, utility, and industrial environments where availability is a key performance requirement. See also: Availability, Reliability, Mean Time Between Failures (MTBF).</p>
    </div>

    <div class="glossary-term" data-category="data-quality maximo">
      <h3 id="operational-data-alignment">Operational Data Alignment</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
      </div>
      <p>Operational Data Alignment is the degree to which data recorded in Maximo accurately reflects what is actually happening in the field — including what work was done, when, by whom, and with what materials. When operational data alignment is high, management can trust Maximo reports to guide decisions. When it is low, there is a gap between the system of record and operational reality, and that gap grows over time as habits and workarounds become entrenched. Improving operational data alignment requires closing the gap between how work is planned in the system and how it is executed and recorded in the field. See also: Execution Alignment, Work Order Data Quality, Data Discipline.</p>
    </div>


    <h2 id="P">P</h2>

    <div class="glossary-term" data-category="strategy">
      <h3 id="pre-commissioning">Pre-Commissioning</h3>
      <div class="glossary-tags">
        <span>Strategy</span>
      </div>
      <p>Pre-Commissioning is the phase of work performed on a new or significantly modified asset before formal commissioning testing begins — including mechanical completion checks, initial cleaning, lubrication, alignment verification, and safety inspections. Pre-commissioning confirms that an asset is physically ready for the functional testing that commissioning requires. For plant managers and reliability professionals, pre-commissioning is often where data capture disciplines are established: asset records created in Maximo, initial condition documented, and PM programs loaded before the asset enters service. Skipping or compressing pre-commissioning to accelerate startup often creates problems that take years to untangle. See also: Commissioning, Asset Baseline, Asset Acquisition.</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="planned-vs-unplanned-work">Planned vs. Unplanned Work</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Planned vs. Unplanned Work is a ratio that measures the proportion of maintenance activity that was anticipated and prepared in advance versus work that was triggered by unexpected failures or urgent requests. A high planned work percentage indicates a proactive, reliability-focused maintenance organization. A high unplanned work percentage indicates a reactive one — where resources are consumed responding to failures rather than preventing them. Most mature maintenance organizations target 80% or more planned work. Tracking this ratio in Maximo requires consistent Work Type classification and disciplined work order management. See also: Work Type, Reactive Work, Backlog Health, Planning and Scheduling.</p>
    </div>

    <div class="glossary-term" data-category="maintenance analytics">
      <h3 id="planning-accuracy">Planning Accuracy</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Maintenance</span>
      </div>
      <p>Planning Accuracy measures how closely the estimated labor hours, materials, and durations on a work order match what was actually required to complete the work. High planning accuracy reduces scheduling conflicts, improves resource utilization, and builds trust between planners and the field. Low planning accuracy — where estimates consistently miss actual requirements — leads to schedule instability, resource shortages, and frustration. Improving planning accuracy requires analyzing the gap between planned and actual data in Maximo over time, which is only possible when work order closeout data is captured consistently. See also: Job Plan, Work Order Data Quality, Execution Alignment.</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy">
      <h3 id="planning-and-scheduling">Planning and Scheduling</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Planning and Scheduling is the two-stage process of defining what work needs to be done and how (planning) and then assigning when, where, and by whom it will be executed (scheduling). Planning and scheduling are distinct activities and are most effective when handled by dedicated roles — a planner develops the work package, a scheduler builds the work plan. In Maximo, the planning and scheduling process is supported through work order management, Job Plans, labor assignment, and crew scheduling. Organizations that skip or compress planning often find themselves reactive, over-extended, and unable to improve because they have no history of what good work preparation looks like. See also: Job Plan, Planning Accuracy, Planned vs. Unplanned Work.</p>
    </div>

    <div class="glossary-term" data-category="analytics reliability integration">
      <h3 id="predictive-analytics">Predictive Analytics</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Integration</span>
        <span>Reliability</span>
      </div>
      <p>Predictive Analytics uses statistical models, machine learning, and historical data to anticipate future asset behavior — identifying likely failure patterns, estimating remaining useful life, and forecasting when maintenance intervention will be needed. In the context of IBM MAS, Maximo Predict applies predictive analytics to asset condition and maintenance history data to generate failure probability scores and maintenance recommendations. The quality of predictive analytics output depends heavily on the quality and completeness of the historical data feeding the models — predictions built on poor maintenance history will be unreliable. See also: Predictive Maintenance (PdM), Remaining Useful Life (RUL), Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="maintenance analytics integration">
      <h3 id="predictive-maintenance-pdm">Predictive Maintenance (PdM)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Integration</span>
        <span>Maintenance</span>
      </div>
      <p>Predictive Maintenance is a maintenance strategy that uses condition data, sensor readings, and analytical models to anticipate asset failures before they occur, allowing maintenance to be triggered by predicted risk rather than fixed schedules or observed thresholds. PdM builds on Condition-Based Maintenance (CBM) by going a step further: CBM responds when a condition threshold is crossed, while PdM uses models to forecast when that threshold will be crossed before it happens. Calling a time-based PM schedule "predictive" because it runs in a CMMS is a common and significant misuse of the term. Predictive Maintenance requires real-time or near-real-time condition data, analytical capability, and integration with work management to close the loop from prediction to action. See also: Condition-Based Maintenance (CBM), Preventive Maintenance (PM), Condition Monitoring.</p>
    </div>

    <div class="glossary-term" data-category="maintenance analytics">
      <h3 id="prescriptive-maintenance">Prescriptive Maintenance</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Maintenance</span>
      </div>
      <p>Prescriptive Maintenance is an advanced maintenance approach that goes beyond predicting when a failure is likely to occur — it recommends the specific maintenance action to take, when to take it, and what resources are required. Where Predictive Maintenance says "this asset is likely to fail within 14 days," Prescriptive Maintenance adds "here is the intervention recommended to prevent it and when to schedule it." Prescriptive capabilities are emerging in platforms like IBM MAS through AI-driven recommendation engines. Realizing prescriptive maintenance requires both mature condition monitoring data and a well-governed work management process to act on recommendations consistently. See also: Predictive Maintenance (PdM), Condition Monitoring, Maximo Application Suite (MAS).</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="preventive-maintenance-pm">Preventive Maintenance (PM)</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Preventive Maintenance is scheduled maintenance performed at defined time or usage intervals — regardless of observed asset condition — to reduce the likelihood of failure and sustain reliable operation. PMs are managed in Maximo through PM records that generate work orders automatically based on frequency triggers. Preventive Maintenance is often confused with Predictive Maintenance, but they are fundamentally different: Preventive is interval-driven; Predictive is condition- and data-driven. Not every asset benefits from a preventive schedule — for some assets, a run-to-failure or condition-based approach is more appropriate. PM optimization — regularly reviewing whether PM tasks and frequencies are still justified — is an important part of a mature reliability strategy. See also: Predictive Maintenance (PdM), Condition-Based Maintenance (CBM), PM Compliance.</p>
    </div>

    <div class="glossary-term" data-category="maintenance reliability governance">
      <h3 id="pm-compliance">Preventive Maintenance (PM) Compliance</h3>
      <div class="glossary-tags">
        <span>Governance</span>
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Preventive Maintenance Compliance measures the percentage of scheduled PM work orders that are completed within their defined window, indicating how consistently the maintenance team executes the planned reliability program. PM compliance is one of the most commonly tracked maintenance KPIs — and one of the most commonly misread. A high compliance rate built on PM tasks that are outdated, unnecessary, or poorly designed does not indicate a healthy reliability program. Compliance should be evaluated alongside PM quality and the validity of the underlying PM strategy, not just as a standalone percentage. Maximo supports PM compliance tracking through work order completion dates and PM schedule records. See also: Preventive Maintenance (PM), Key Performance Indicator (KPI), Reliability Strategy.</p>
    </div>


    <h2 id="R">R</h2>

    <div class="glossary-term" data-category="maintenance reliability">
      <h3 id="reactive-work">Reactive Work</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Reliability</span>
      </div>
      <p>Reactive Work is unplanned maintenance performed in response to an unexpected asset failure or urgent condition, restoring operation but consuming resources that could have been deployed on planned work. Reactive work is not the same as Corrective Maintenance — corrective maintenance can be planned and intentional. Reactive work is always unplanned and disruptive. A high proportion of reactive work is a leading indicator of an immature maintenance program — it signals that failures are not being anticipated, that PM strategies may be inadequate, or that asset health is deteriorating faster than planned maintenance can address. Reducing reactive work is a primary goal of reliability strategy. See also: Corrective Maintenance (CM), Planned vs. Unplanned Work, Reliability Strategy.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="reliability">Reliability</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Reliability is the probability that an asset will perform its required function under defined conditions for a specified period without failure. In reliability engineering, Reliability and Availability are precise and distinct metrics. Reliability measures the likelihood of failure-free operation during a defined period. Availability measures the proportion of total time an asset is operational, including the impact of both scheduled and unscheduled downtime. An asset can be highly reliable — rarely failing unexpectedly — but still have low availability if it is frequently taken offline for planned maintenance. Treating these as the same number in KPI reporting leads to poor decisions about maintenance strategy and capital investment. See also: Availability, Operational Availability (Ao), Mean Time Between Failures (MTBF).</p>
    </div>

    <div class="glossary-term" data-category="reliability strategy governance">
      <h3 id="reliability-strategy">Reliability Strategy</h3>
      <div class="glossary-tags">
        <span>Governance</span>
        <span>Reliability</span>
        <span>Strategy</span>
      </div>
      <p>Reliability Strategy is the organizational plan that defines how maintenance work will be designed and deployed to manage asset risk and sustain performance — determining what maintenance tasks are performed, how often, and by what method for each asset class. A mature reliability strategy is not a single approach applied uniformly; it is a deliberate mix of preventive, predictive, condition-based, and run-to-failure strategies selected based on asset criticality, failure mode characteristics, and operational context. Without a defined reliability strategy, maintenance programs default to habit and reaction rather than evidence-based decision-making. Maximo enables reliability strategy execution through PM records, Job Plans, failure coding, and condition monitoring — but the strategy must come first. See also: Asset Criticality, Preventive Maintenance (PM), Predictive Maintenance (PdM), Failure Mode.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="remaining-useful-life-rul">Remaining Useful Life (RUL)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Remaining Useful Life (RUL) is an estimate of how much longer an asset can continue to operate before it is expected to fail or require replacement, based on current condition, historical performance, and usage data. RUL estimates help reliability and capital planning teams prioritize maintenance investment, schedule major repairs or replacements before failure, and avoid both premature replacement and run-to-failure surprises. In IBM MAS, Maximo Health and Maximo Predict can generate RUL estimates from condition data and failure history. The accuracy of RUL estimates depends on the quality of the underlying data and the appropriateness of the model for the asset type. See also: Asset Health Index (AHI), Predictive Analytics, Asset Lifecycle Cost, Lifecycle Replacement Decision.</p>
    </div>

    <div class="glossary-term" data-category="reliability strategy">
      <h3 id="run-to-failure-rtf">Run-to-Failure (RTF)</h3>
      <div class="glossary-tags">
        <span>Reliability</span>
        <span>Strategy</span>
      </div>
      <p>Run-to-Failure (RTF) is an intentional maintenance strategy in which no proactive maintenance is performed on an asset — it is allowed to operate until it fails, at which point it is repaired or replaced. RTF is not a default or a sign of neglect; for the right assets, it is the most cost-effective strategy. RTF is appropriate for non-critical assets where failure has no safety or operational consequence, redundancy exists, and the cost of preventive maintenance exceeds the cost of failure. For reliability professionals, identifying which assets are appropriate RTF candidates — and making that decision explicitly rather than by omission — is an important part of maintenance strategy design. Unintentional RTF on critical assets, by contrast, is one of the most costly failures of a reliability program. See also: Reliability Strategy, Asset Criticality, Preventive Maintenance (PM), End-of-Life (EOL).</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="lifecycle-replacement-decision">Lifecycle Replacement Decision</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>A Lifecycle Replacement Decision is the structured evaluation of whether to continue maintaining an aging or degraded asset or to replace it — weighing the cost and risk of continued operation against the capital and operational cost of acquiring and commissioning a new asset. This decision is one of the most consequential in asset management and is often made poorly — either replacing assets prematurely out of caution or running them far past the point where continued investment makes economic sense. For plant managers and reliability professionals, a defensible replacement decision requires condition data, maintenance cost history, remaining useful life estimates, and lifecycle cost projections — the kind of evidence that a well-governed Maximo implementation is designed to provide. See also: Remaining Useful Life (RUL), Asset Lifecycle Cost, Total Cost of Ownership (TCO), End-of-Life (EOL), Life Extension.</p>
    </div>

    <div class="glossary-term" data-category="reliability strategy">
      <h3 id="life-extension">Life Extension</h3>
      <div class="glossary-tags">
        <span>Reliability</span>
        <span>Strategy</span>
      </div>
      <p>Life Extension is a deliberate strategy to extend the operating life of an asset beyond its original design life or planned retirement date through targeted investment in major overhauls, component replacement, upgrades, or condition-based interventions. Life extension decisions require careful analysis — the cost of extending an asset's life must be weighed against the cost and benefit of replacement, and the risks of continued operation must be understood and managed. For reliability professionals, life extension programs require updated condition assessments, revised PM strategies, and often enhanced monitoring to manage the higher failure risk that accompanies aging assets. For plant managers, life extension can defer significant CapEx but should be treated as a deliberate decision, not a default. See also: Lifecycle Replacement Decision, Asset Lifecycle Cost, Remaining Useful Life (RUL), Capital Expenditure (CapEx).</p>
    </div>

    <div class="glossary-term" data-category="maximo troubleshooting">
      <h3 id="residual-state">Residual State</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>Residual State is the condition left in Maximo after a failed or incomplete operation, where internal system flags, status fields, or lock indicators reflect a prior or partially completed action rather than the actual current state of the record. Residual state issues often manifest as records that appear locked, status transitions that fail without clear error messages, or workflows that do not advance as expected. Resolving residual state typically requires identifying and correcting the underlying system flags rather than repeating the failed action. Understanding residual state is essential for Maximo administrators troubleshooting intermittent or hard-to-reproduce application behavior. See also: Mid-Transaction Failure, Transaction Rollback, System Record Integrity.</p>
    </div>

    <div class="glossary-term" data-category="reliability analytics">
      <h3 id="root-cause-analysis-rca">Root Cause Analysis (RCA)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Reliability</span>
      </div>
      <p>Root Cause Analysis (RCA) is a structured investigation method used to identify the fundamental cause of a failure — not just the immediate symptom — so that corrective actions can prevent recurrence rather than simply restoring operation. RCA is most valuable when applied to significant failures, recurring failure patterns, and high-consequence events. Effective RCA requires good failure data — accurate failure codes, complete work order history, and documented symptoms and conditions — which makes Maximo data quality a prerequisite for meaningful analysis. Without reliable failure history, RCA becomes guesswork. See also: Failure Mode, Failure Code, Failure Data Quality.</p>
    </div>


    <h2 id="S">S</h2>

    <div class="glossary-term" data-category="governance strategy">
      <h3 id="service-level-agreement-sla">Service Level Agreement (SLA)</h3>
      <div class="glossary-tags">
        <span>Governance</span>
        <span>Strategy</span>
      </div>
      <p>A Service Level Agreement (SLA) is a documented commitment that defines expected performance standards for a service — including response times, resolution targets, and quality criteria — creating clear accountability between service providers and their customers or stakeholders. In a maintenance context, SLAs may define how quickly different classes of work requests must be acknowledged, planned, and completed. In Maximo, SLA tracking can be configured to monitor response and resolution times against defined targets. SLAs are only meaningful when the underlying data is captured accurately enough to measure compliance. See also: Key Performance Indicator (KPI), Work Request.</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy">
      <h3 id="spare-parts-strategy-commissioning">Spare Parts Strategy at Commissioning</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Spare Parts Strategy at Commissioning is the process of identifying, procuring, and stocking the initial set of spare parts required to support a new asset before it enters service — based on the asset's criticality, failure modes, lead times for replacement parts, and the operational consequence of downtime. Establishing a spare parts strategy at commissioning is significantly more effective than trying to build it reactively after the first failure reveals a gap. For plant managers and reliability professionals, commissioning is the moment to load stocking requirements into Maximo, establish reorder points, and ensure critical spares are on the shelf before the asset is needed. Deferring this work almost always results in extended downtime during the first major failure event. See also: Commissioning, Asset Criticality, Inventory Optimization.</p>
    </div>

    <div class="glossary-term" data-category="strategy analytics">
      <h3 id="asset-write-off">Asset Write-Off</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>An Asset Write-Off is the formal accounting and system process of removing a retired or disposed asset's remaining book value from the balance sheet and closing its record in the asset management system. Write-offs are the financial bookend to the asset lifecycle — they recognize that the asset no longer has value or is no longer in service. In Maximo, completing a write-off properly means retiring the asset record, closing open work orders, removing the asset from active PM schedules, and preserving its history in archived form. Assets that are physically gone but still active in Maximo inflate asset counts, distort maintenance metrics, and create inventory planning errors for parts that are no longer needed. See also: Asset Disposal, Decommissioning, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="maintenance maximo mobile">
      <h3 id="standard-job-plan">Standard Job Plan</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
        <span>Mobile</span>
      </div>
      <p>A Standard Job Plan in Maximo is a reusable work template that defines the standard way a recurring maintenance task should be completed, including task steps, labor requirements, and materials. Standard Job Plans are applied to PM records so that every work order generated for that task inherits a consistent, pre-built work package. They reduce planning time, improve consistency across shifts and crews, and produce comparable work order data that can be analyzed over time. The distinction between a Job Plan and a Standard Job Plan is primarily in how they are applied — Standard Job Plans are specifically designed to support recurring, scheduled work. See also: Job Plan, Preventive Maintenance (PM), Planning Accuracy.</p>
    </div>

    <div class="glossary-term" data-category="data-quality reliability governance">
      <h3 id="standardized-failure-codes">Standardized Failure Codes</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Governance</span>
        <span>Reliability</span>
      </div>
      <p>Standardized Failure Codes are a governed set of classification descriptors — typically covering problem, cause, and remedy — used consistently across the organization to record how and why assets fail. Standardization is what makes failure codes analytically useful: if different technicians or sites use different codes for the same failure, or apply the same code to different failures, the resulting data cannot be aggregated or compared. Building a standardized failure code taxonomy requires input from reliability engineers and operations teams, and sustaining it requires governance, training, and ongoing review. See also: Failure Code, Failure Data Quality, Data Governance.</p>
    </div>

    <div class="glossary-term" data-category="maximo data-quality troubleshooting">
      <h3 id="system-record-integrity">System Record Integrity</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>System Record Integrity is the accuracy and internal consistency of Maximo's configuration and data records — including application definitions, workflow configurations, relationship tables, and system flags — that application logic, integrations, and dependent processes rely on to function correctly. When system record integrity is compromised — through incomplete migrations, failed transactions, or unsupported customizations — Maximo can exhibit unpredictable behavior that is difficult to diagnose because the visible application state does not reflect the underlying system state. Maintaining system record integrity is a responsibility of Maximo administrators and is particularly important during upgrades and data migrations. See also: Residual State, Mid-Transaction Failure, Transaction Rollback.</p>
    </div>


    <h2 id="T">T</h2>

    <div class="glossary-term" data-category="analytics strategy">
      <h3 id="total-cost-of-ownership-tco">Total Cost of Ownership (TCO)</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Strategy</span>
      </div>
      <p>Total Cost of Ownership is the complete cost of an asset across its entire lifecycle, including acquisition, installation, operation, maintenance, and disposal. TCO is broader than Maintenance Cost, which covers only the expense of keeping an asset running. An asset that is inexpensive to maintain may still carry poor TCO if it is costly to operate, energy-intensive, or expensive to decommission. Organizations that focus only on reducing maintenance spend often underestimate true asset investment and make capital decisions that look good on a maintenance budget but are poor choices from a lifecycle perspective. TCO analysis is a key input to capital planning, replacement decisions, and lifecycle strategy. See also: Asset Lifecycle Cost, Maintenance Cost, Asset Lifecycle.</p>
    </div>

    <div class="glossary-term" data-category="maximo troubleshooting">
      <h3 id="transaction-rollback">Transaction Rollback</h3>
      <div class="glossary-tags">
        <span>Maximo</span>
        <span>Troubleshooting</span>
      </div>
      <p>A Transaction Rollback is the automatic or manual reversal of a database operation that failed to complete successfully, returning the affected records to their prior consistent state and preventing partial changes from persisting in the system. In Maximo, rollbacks are part of the database transaction management layer — when an operation fails, the system attempts to roll back all changes made within that transaction. When a rollback does not complete cleanly, it can result in residual state issues that require manual investigation and correction. Understanding when rollbacks occur and how to identify their aftermath is important for Maximo administrators managing system stability. See also: Mid-Transaction Failure, Residual State, System Record Integrity.</p>
    </div>


    <h2 id="U">U</h2>

    <div class="glossary-term" data-category="data-quality analytics">
      <h3 id="usable-data">Usable Data</h3>
      <div class="glossary-tags">
        <span>Analytics</span>
        <span>Data Quality</span>
      </div>
      <p>Usable Data is information in Maximo that is sufficiently complete, consistent, and structured to support the decisions, analysis, and planning it was intended to enable. Data can exist in Maximo without being usable — work orders with blank failure codes, assets without hierarchy, labor transactions without actual hours. The gap between data that has been entered and data that is actually usable is one of the most common and costly problems in Maximo implementations. Usable data is the output of disciplined data governance, consistent standards, and accountable work management practices. See also: Data Quality, Data Confidence, Data Discipline.</p>
    </div>


    <h2 id="W">W</h2>

    <div class="glossary-term" data-category="maintenance strategy governance">
      <h3 id="work-management-consistency">Work Management Consistency</h3>
      <div class="glossary-tags">
        <span>Governance</span>
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Work Management Consistency is the degree to which work is planned, executed, documented, and closed in the same way — using the same standards, workflows, and data entry practices — across shifts, crews, sites, and time. Consistency is what makes work management data comparable and analytically useful. Without it, one crew's "PM completed" looks identical in the system to another crew's "PM skipped and closed anyway," and management cannot tell the difference. Building consistency requires clear standards, embedded workflow controls in Maximo, supervisory reinforcement, and accountability for data quality at the point of entry. See also: Work Management Discipline, Data Discipline, Execution Alignment.</p>
    </div>

    <div class="glossary-term" data-category="maintenance strategy governance">
      <h3 id="work-management-discipline">Work Management Discipline</h3>
      <div class="glossary-tags">
        <span>Governance</span>
        <span>Maintenance</span>
        <span>Strategy</span>
      </div>
      <p>Work Management Discipline is the organizational habit of following defined work management processes consistently — planning work before it starts, documenting what was done during execution, and capturing required data at closeout — making maintenance activity predictable, measurable, and improvable over time. Discipline is distinct from process: an organization can have excellent documented processes and poor discipline if those processes are not consistently followed. Work management discipline is the behavioral foundation that determines whether Maximo investment produces reliable data and meaningful reporting. See also: Work Management Consistency, Data Discipline, Execution Alignment.</p>
    </div>

    <div class="glossary-term" data-category="maximo maintenance mobile">
      <h3 id="work-order-wo">Work Order (WO)</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
        <span>Mobile</span>
      </div>
      <p>A Work Order in Maximo is the primary record used to plan, authorize, execute, and document a maintenance task, capturing the scope of work, assigned labor, required materials, actual costs, and completion details. Work orders are the central unit of work management in Maximo — they are the source of maintenance history, the input to failure analysis, and the basis for cost reporting. A Work Order is not the same as a Work Request. A Work Request is an initial notification that something needs attention. A Work Order is an authorized, planned, and resourced task. Skipping the discipline of converting requests into properly planned work orders is one of the most common reasons Maximo data quality degrades over time. See also: Work Request, Job Plan, Work Order Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="maintenance data-quality mobile">
      <h3 id="work-order-closeout">Work Order Closeout</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maintenance</span>
        <span>Mobile</span>
      </div>
      <p>Work Order Closeout is the process of completing a work order in Maximo with all required data after the maintenance task is finished, including actual labor hours, materials used, failure codes, work performed descriptions, and any follow-up actions identified. Closeout is where the value of the work management process is either captured or lost — a work order closed with complete, accurate data contributes to a reliable maintenance history; one closed with missing or generic entries adds noise that undermines analysis. In Maximo Mobile, closeout is completed in the field, making mobile usability and clear expectations critical to closeout quality. See also: Closeout Quality, Work Order Data Quality, Failure Code.</p>
    </div>

    <div class="glossary-term" data-category="maintenance data-quality">
      <h3 id="work-order-closeout-quality">Work Order Closeout Quality</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maintenance</span>
      </div>
      <p>Work Order Closeout Quality is the consistency and completeness with which required information is captured when work orders are finished — including failure codes, actual labor, materials consumed, and work descriptions. Closeout quality is the single biggest determinant of how useful Maximo maintenance history is for reliability analysis, cost reporting, and PM optimization. It is also one of the hardest data quality dimensions to sustain, because it depends on the habits of every technician closing every work order — under time pressure, at the end of a shift, or in the field on a mobile device. See also: Work Order Closeout, Closeout Quality, Failure Code.</p>
    </div>

    <div class="glossary-term" data-category="maintenance data-quality">
      <h3 id="work-order-data-quality">Work Order Data Quality</h3>
      <div class="glossary-tags">
        <span>Data Quality</span>
        <span>Maintenance</span>
      </div>
      <p>Work Order Data Quality is the overall completeness, accuracy, and consistency of information captured across the work order lifecycle in Maximo — from creation and planning through execution and closeout. Work order data is the primary source of maintenance history, and its quality determines whether that history can support failure analysis, cost tracking, PM optimization, and reliability reporting. Poor work order data quality is extremely common and often invisible until an organization tries to use the data for analysis and finds it unreliable. Improving it requires addressing both the structural factors (standards, required fields, workflows) and the behavioral factors (training, accountability, leadership reinforcement). See also: Closeout Quality, Work Order Closeout Quality, Failure Code, Data Quality.</p>
    </div>

    <div class="glossary-term" data-category="maximo maintenance">
      <h3 id="work-request">Work Request</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
      </div>
      <p>A Work Request is an initial notification submitted to the maintenance team indicating that a problem has been identified or that work may be needed — submitted by anyone who observes an issue, not just maintenance personnel. A Work Request is a trigger, not an authorization. It becomes a Work Order only after it has been reviewed, prioritized, approved, planned, and resourced by the maintenance planning function. Maintaining the distinction between requests and work orders is fundamental to data quality and planning discipline in Maximo — collapsing the two, or allowing work to be executed directly from requests without proper planning, undermines backlog visibility, resource management, and maintenance history. See also: Work Order (WO), Backlog Health, Planning and Scheduling.</p>
    </div>

    <div class="glossary-term" data-category="maximo maintenance">
      <h3 id="maximo-work-type">Work Type</h3>
      <div class="glossary-tags">
        <span>Maintenance</span>
        <span>Maximo</span>
      </div>
      <p>Work Type is a Maximo classification field on the work order that categorizes the nature of the maintenance activity — such as Preventive Maintenance, Corrective Maintenance, Emergency, or Inspection — helping route work through appropriate workflows and enabling reporting on how maintenance resources are distributed across work categories. Work Type is one of the most important fields for measuring planned versus unplanned work ratios and evaluating the overall health of the maintenance program. When Work Type is applied inconsistently or defaulted without thought, the resulting data cannot accurately represent how the maintenance team is spending its time. See also: Planned vs. Unplanned Work, Corrective Maintenance (CM), Preventive Maintenance (PM).</p>
    </div>


  </div>
</div>

<style>
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0,0,0,0);
  white-space: nowrap;
  border: 0;
}

.glossary-shell {
  margin-top: 24px;
}

.glossary-toolbar {
  display: flex;
  gap: 16px;
  justify-content: space-between;
  align-items: center;
  margin: 0 0 14px;
  flex-wrap: wrap;
}

.glossary-search-wrap {
  flex: 1 1 380px;
}

.glossary-search {
  width: 100%;
  min-height: 48px;
  padding: 12px 16px;
  border: 1px solid var(--border);
  border-radius: 12px;
  background: var(--white);
  font-size: 16px;
  color: var(--maven-blue-deep);
  box-shadow: 0 6px 16px rgba(41, 44, 117, 0.06);
}

.glossary-search:focus {
  outline: none;
  border-color: var(--maven-blue-primary);
  box-shadow: 0 0 0 3px rgba(62, 103, 177, 0.12);
}

.glossary-meta {
  display: flex;
  align-items: center;
  gap: 12px;
  color: var(--text-muted, #5d6475);
  font-size: 14px;
}

.glossary-clear {
  border: 1px solid var(--border);
  background: var(--white);
  color: var(--maven-blue-deep);
  border-radius: 999px;
  padding: 8px 14px;
  font-size: 14px;
  cursor: pointer;
}

.glossary-clear:hover {
  border-color: var(--maven-blue-primary);
}

.glossary-filters {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 18px;
}

.glossary-filter {
  border: 1px solid var(--border);
  background: var(--white);
  color: var(--maven-blue-deep);
  border-radius: 999px;
  padding: 9px 14px;
  font-size: 14px;
  cursor: pointer;
  transition: all 0.2s ease;
}

.glossary-filter:hover,
.glossary-filter.is-active {
  background: var(--maven-blue-deep);
  color: #fff;
  border-color: var(--maven-blue-deep);
}

.glossary-nav {
  position: sticky;
  top: 14px;
  z-index: 9999;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin: 18px 0 30px;
  padding: 14px 16px;
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: 14px;
  box-shadow: 0 10px 26px rgba(41, 44, 117, 0.10);
}

.glossary-nav a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-width: 34px;
  height: 34px;
  padding: 0 10px;
  border-radius: 999px;
  font-size: 13px;
  font-weight: 700;
  text-decoration: none;
  color: var(--maven-blue-deep);
  background: rgba(62, 103, 177, 0.08);
  border: 1px solid transparent;
  transition: background 0.2s ease, color 0.2s ease, border-color 0.2s ease, transform 0.15s ease, box-shadow 0.2s ease;
}

.glossary-nav a:hover {
  background: var(--maven-blue-primary);
  color: #fff;
  border-color: var(--maven-blue-primary);
  transform: translateY(-1px);
  box-shadow: 0 6px 14px rgba(62, 103, 177, 0.25);
}

.glossary h2,
.glossary-term h3,
#top {
  scroll-margin-top: 110px;
}

.glossary-term {
  margin: 0 0 18px;
  padding: 0 0 18px;
  border-bottom: 1px solid var(--border);
}

.glossary-term h3 {
  margin-bottom: 8px;
}

.glossary-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin: 0 0 10px;
}

.glossary-tags span {
  display: inline-flex;
  align-items: center;
  min-height: 28px;
  padding: 4px 10px;
  border-radius: 999px;
  background: rgba(62, 103, 177, 0.08);
  color: var(--maven-blue-deep);
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 0.01em;
}

.glossary-empty {
  display: block;
  padding: 18px 20px;
  border: 1px dashed var(--border);
  border-radius: 12px;
  margin: 12px 0 22px;
  color: var(--text-muted, #5d6475);
  background: rgba(62, 103, 177, 0.03);
}

.glossary-letter-hidden {
  display: none;
}

.glossary-term-hidden {
  display: none;
}

@media (max-width: 640px) {
  .glossary-nav {
    padding: 12px;
    gap: 6px;
    top: 8px;
  }

  .glossary-nav a {
    min-width: 30px;
    height: 30px;
    font-size: 12px;
  }

  .glossary-meta {
    width: 100%;
    justify-content: space-between;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function () {
  const searchInput = document.getElementById('glossary-search');
  const clearButton = document.getElementById('glossary-clear');
  const countEl = document.getElementById('glossary-count');
  const emptyEl = document.getElementById('glossary-empty');
  const filtersWrap = document.getElementById('glossary-filters');
  const terms = Array.from(document.querySelectorAll('.glossary-term'));
  const headings = Array.from(document.querySelectorAll('.glossary h2'));

  let activeFilter = 'all';

  function normalize(text) {
    return (text || '').toLowerCase().trim();
  }

  function slugToLabel(slug) {
    return slug
      .split('-')
      .map(part => part.charAt(0).toUpperCase() + part.slice(1))
      .join(' ');
  }

  function labelToSlug(label) {
    return normalize(label).replace(/\s+/g, '-');
  }

  function sortAndNormalizeTermCategories() {
    terms.forEach(term => {
      const tagContainer = term.querySelector('.glossary-tags');
      if (!tagContainer) return;

      const tags = Array.from(tagContainer.querySelectorAll('span'));

      tags.sort((a, b) => a.textContent.localeCompare(b.textContent));

      tagContainer.innerHTML = '';
      tags.forEach(tag => tagContainer.appendChild(tag));

      const sortedSlugs = tags.map(tag => labelToSlug(tag.textContent));
      term.dataset.category = sortedSlugs.join(' ');
    });
  }

  function collectCategories() {
    const categorySet = new Set();

    terms.forEach(term => {
      const raw = normalize(term.dataset.category);
      if (!raw) return;

      raw.split(/\s+/).forEach(cat => {
        if (cat) categorySet.add(cat);
      });
    });

    return Array.from(categorySet).sort((a, b) => a.localeCompare(b));
  }

  function renderFilterButtons() {
    const categories = collectCategories();

    filtersWrap.innerHTML = '';

    const allButton = document.createElement('button');
    allButton.type = 'button';
    allButton.className = 'glossary-filter is-active';
    allButton.dataset.filter = 'all';
    allButton.textContent = 'All';
    filtersWrap.appendChild(allButton);

    categories.forEach(category => {
      const button = document.createElement('button');
      button.type = 'button';
      button.className = 'glossary-filter';
      button.dataset.filter = category;
      button.textContent = slugToLabel(category);
      filtersWrap.appendChild(button);
    });
  }

  function getFilterButtons() {
    return Array.from(document.querySelectorAll('.glossary-filter'));
  }

  function updateGlossary() {
    const query = normalize(searchInput.value);
    let visibleCount = 0;

    terms.forEach(term => {
      const text = normalize(term.textContent);
      const categories = normalize(term.dataset.category);
      const matchesSearch = !query || text.includes(query);
      const matchesFilter = activeFilter === 'all' || categories.split(/\s+/).includes(activeFilter);
      const show = matchesSearch && matchesFilter;

      term.classList.toggle('glossary-term-hidden', !show);

      if (show) visibleCount += 1;
    });

    headings.forEach(heading => {
      let next = heading.nextElementSibling;
      let hasVisibleTerms = false;

      while (next && next.tagName !== 'H2') {
        if (next.classList.contains('glossary-term') && !next.classList.contains('glossary-term-hidden')) {
          hasVisibleTerms = true;
          break;
        }
        next = next.nextElementSibling;
      }

      heading.classList.toggle('glossary-letter-hidden', !hasVisibleTerms);
    });

    countEl.textContent = visibleCount === 1 ? '1 term' : visibleCount + ' terms';
    emptyEl.hidden = visibleCount !== 0;
  }

  function bindFilterEvents() {
    getFilterButtons().forEach(button => {
      button.addEventListener('click', function () {
        getFilterButtons().forEach(btn => btn.classList.remove('is-active'));
        button.classList.add('is-active');
        activeFilter = button.dataset.filter;
        updateGlossary();
      });
    });
  }

  clearButton.addEventListener('click', function () {
    searchInput.value = '';
    activeFilter = 'all';
    getFilterButtons().forEach(btn => btn.classList.remove('is-active'));
    const allButton = document.querySelector('.glossary-filter[data-filter="all"]');
    if (allButton) allButton.classList.add('is-active');
    updateGlossary();
    searchInput.focus();
  });

  searchInput.addEventListener('input', updateGlossary);

  sortAndNormalizeTermCategories();
  renderFilterButtons();
  bindFilterEvents();
  updateGlossary();
});
</script>
