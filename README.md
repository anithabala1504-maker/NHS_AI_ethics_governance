<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>CPI AI Governance Checklist</title>

<style>
body {font-family: Arial; background:#f9fafc; margin:20px;}
h1 {color:#003087;}
.section {margin-bottom:25px; background:white; padding:15px; border-radius:8px;}
.item {border:1px solid #ddd; padding:10px; margin-bottom:8px; border-radius:6px;}
.item-title {font-weight:bold; margin-bottom:4px;}
.pill {padding:3px 8px; border-radius:10px; font-size:11px; margin-right:5px;}
.mandatory {background:#ffdede;}
.recommended {background:#e7f7e7;}
.high {background:#ffe6cc;}
.medium {background:#fff7cc;}
.low {background:#e6ffe6;}
.status {margin-top:5px;}
button {margin-top:5px; padding:2px 6px;}
</style>

<script>
function updateStatus(id, status) {
  document.getElementById("status-"+id).innerText = status;

  let rag = "";
  if(status=="Complete") rag="🟢 Green";
  else if(status=="In Progress") rag="🟠 Amber";
  else rag="🔴 Red";

  document.getElementById("rag-"+id).innerText = rag;
}
</script>
</head>

<body>

<h1>CPI AI Governance Checklist (NHS Cancer Diagnostics)</h1>

<!-- SECTION 1 -->
<div class="section">
<h2>1. Clinical Context</h2>

<div class="item">
<div class="item-title">Define intended clinical purpose</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Intended Use Document</div>
<div class="status">Status: <span id="status-C1"></span></div>
<div>RAG: <span id="rag-C1"></span></div>
<button onclick="updateStatus('C1','Complete')">Complete</button>
<button onclick="updateStatus('C1','In Progress')">In Progress</button>
<button onclick="updateStatus('C1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 2 -->
<div class="section">
<h2>2. Medical Device Compliance (MHRA)</h2>

<div class="item">
<div class="item-title">Classify AI as SaMD</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: MHRA Classification Record</div>
<div>Status: <span id="status-M1"></span></div>
<div>RAG: <span id="rag-M1"></span></div>
<button onclick="updateStatus('M1','Complete')">Complete</button>
<button onclick="updateStatus('M1','In Progress')">In Progress</button>
<button onclick="updateStatus('M1','Not Started')">Not Started</button>
</div>

<div class="item">
<div class="item-title">Create Post-Market Surveillance Plan</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: PMS Plan</div>
<div>Status: <span id="status-M2"></span></div>
<div>RAG: <span id="rag-M2"></span></div>
<button onclick="updateStatus('M2','Complete')">Complete</button>
<button onclick="updateStatus('M2','In Progress')">In Progress</button>
<button onclick="updateStatus('M2','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 3 -->
<div class="section">
<h2>3. UK GDPR & Data Governance</h2>

<div class="item">
<div class="item-title">Complete DPIA</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Signed DPIA</div>
<div>Status: <span id="status-D1"></span></div>
<div>RAG: <span id="rag-D1"></span></div>
<button onclick="updateStatus('D1','Complete')">Complete</button>
<button onclick="updateStatus('D1','In Progress')">In Progress</button>
<button onclick="updateStatus('D1','Not Started')">Not Started</button>
</div>

<div class="item">
<div class="item-title">Define lawful basis</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Legal basis document</div>
<div>Status: <span id="status-D2"></span></div>
<div>RAG: <span id="rag-D2"></span></div>
<button onclick="updateStatus('D2','Complete')">Complete</button>
<button onclick="updateStatus('D2','In Progress')">In Progress</button>
<button onclick="updateStatus('D2','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 4 -->
<div class="section">
<h2>4. Clinical Safety (DCB0129 / DCB0160)</h2>

<div class="item">
<div class="item-title">Appoint Clinical Safety Officer</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Appointment document</div>
<div>Status: <span id="status-CS1"></span></div>
<div>RAG: <span id="rag-CS1"></span></div>
<button onclick="updateStatus('CS1','Complete')">Complete</button>
<button onclick="updateStatus('CS1','In Progress')">In Progress</button>
<button onclick="updateStatus('CS1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 5 -->
<div class="section">
<h2>5. AI Model Governance</h2>

<div class="item">
<div class="item-title">Bias testing across demographics</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Bias report</div>
<div>Status: <span id="status-AI1"></span></div>
<div>RAG: <span id="rag-AI1"></span></div>
<button onclick="updateStatus('AI1','Complete')">Complete</button>
<button onclick="updateStatus('AI1','In Progress')">In Progress</button>
<button onclick="updateStatus('AI1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 6 -->
<div class="section">
<h2>6. EU AI Act (High Risk)</h2>

<div class="item">
<div class="item-title">Establish risk management system</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Risk framework</div>
<div>Status: <span id="status-EU1"></span></div>
<div>RAG: <span id="rag-EU1"></span></div>
<button onclick="updateStatus('EU1','Complete')">Complete</button>
<button onclick="updateStatus('EU1','In Progress')">In Progress</button>
<button onclick="updateStatus('EU1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 7 -->
<div class="section">
<h2>7. Cyber Security</h2>

<div class="item">
<div class="item-title">Complete DSPT</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: DSPT Submission</div>
<div>Status: <span id="status-CY1"></span></div>
<div>RAG: <span id="rag-CY1"></span></div>
<button onclick="updateStatus('CY1','Complete')">Complete</button>
<button onclick="updateStatus('CY1','In Progress')">In Progress</button>
<button onclick="updateStatus('CY1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 8 -->
<div class="section">
<h2>8. CPI as Provider (Procurement)</h2>

<div class="item">
<div class="item-title">Provide governance documentation to NHS</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Governance pack</div>
<div>Status: <span id="status-SUP1"></span></div>
<div>RAG: <span id="rag-SUP1"></span></div>
<button onclick="updateStatus('SUP1','Complete')">Complete</button>
<button onclick="updateStatus('SUP1','In Progress')">In Progress</button>
<button onclick="updateStatus('SUP1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 9 -->
<div class="section">
<h2>9. Ethics & Transparency</h2>

<div class="item">
<div class="item-title">Inform patients AI is used</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Patient leaflet</div>
<div>Status: <span id="status-ETH1"></span></div>
<div>RAG: <span id="rag-ETH1"></span></div>
<button onclick="updateStatus('ETH1','Complete')">Complete</button>
<button onclick="updateStatus('ETH1','In Progress')">In Progress</button>
<button onclick="updateStatus('ETH1','Not Started')">Not Started</button>
</div>

</div>

<!-- SECTION 10 -->
<div class="section">
<h2>10. Lifecycle & Monitoring</h2>

<div class="item">
<div class="item-title">Monitor performance continuously</div>
<span class="pill mandatory">Mandatory</span>
<span class="pill high">High Risk</span>
<div>Evidence: Monitoring reports</div>
<div>Status: <span id="status-L1"></span></div>
<div>RAG: <span id="rag-L1"></span></div>
<button onclick="updateStatus('L1','Complete')">Complete</button>
<button onclick="updateStatus('L1','In Progress')">In Progress</button>
<button onclick="updateStatus('L1','Not Started')">Not Started</button>
</div>

</div>

</body>
</html>
