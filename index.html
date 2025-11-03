 <!DOCTYPE html>
<html>
<head>
  <title>KITENGELA INTERNATIONAL SCHOOL – CAS Log</title>
  <style>
  
  #toast {
    visibility: hidden;
    min-width: 300px;
    background-color: #111;
    color: #00ff7f; /* green success color */
    text-align: center;
    border-radius: 8px;
    padding: 16px;
    position: fixed;
    z-index: 1000;
    left: 50%;
    bottom: 30px;
    transform: translateX(-50%);
    font-weight: 500;
    box-shadow: 0 0 10px rgba(255, 215, 0, 0.4); /* subtle gold glow */
    opacity: 0;
    transition: opacity 0.5s, bottom 0.5s;
  }

  #toast.show {
    visibility: visible;
    opacity: 1;
    bottom: 50px;
  }

    body {
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      color: #333;
      max-width: 700px;
      margin: 40px auto;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    h2 {
      text-align: center;
      margin-bottom: 20px;
    }
    label {
      font-weight: bold;
      display: block;
      margin-top: 15px;
    }
    input[type="text"],
    input[type="date"],
    input[type="number"],
    textarea,
    select {
      width: 100%;
      padding: 8px;
      margin-top: 6px;
      border: 1px solid #ccc;
      border-radius: 6px;
      box-sizing: border-box;
    }
    textarea { resize: vertical; }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      border: none;
      border-radius: 6px;
      background: #007bff;
      color: white;
      cursor: pointer;
      font-size: 15px;
    }
    button:hover { background: #0056b3; }

    /* Checkbox groups */
    .checkbox-group {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: 6px;
      margin-left: 10px;
      margin-top: 8px;
    }
    .checkbox-group label {
      font-weight: normal;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h2>KITENGELA INTERNATIONAL SCHOOL<br>CAS Diary / Log Form</h2>

  <form id="casForm">
    <!-- Name and Adviser -->
    <label>Student Email / ID</label>
    <input type="text" name="studentId" id="studentId" required>
    <button type="button" onclick="checkHours()">Check My Hours</button>
    <p id="summary"></p>

    <label>Student Name (only first time)</label>
    <input type="text" name="studentName">

    <label>CAS Adviser</label>
    <input type="text" name="casAdviser">

    <!-- Date -->
    <label>Date</label>
    <input type="date" name="date" required>

    <!-- Activity -->
    <label>Activity Title</label>
    <input type="text" name="activityTitle" required>

    <!-- CAS Strand -->
    <label>CAS Strand</label>
    <div class="checkbox-group">
      <label><input type="checkbox" name="casStrand" value="Creativity"> Creativity</label>
      <label><input type="checkbox" name="casStrand" value="Action"> Action</label>
      <label><input type="checkbox" name="casStrand" value="Service"> Service</label>
    </div>

    <!-- Description -->
    <label>Description of the Activity</label>
    <textarea name="description" rows="3" required></textarea>

    <!-- Learning Outcomes -->
    <label>Learning Outcomes Addressed</label>
    <p>(Tick all that apply)</p>
    <div class="checkbox-group">
      <label><input type="checkbox" name="learningOutcomes" value="Identify own strengths and develop areas for growth"> Identify own strengths and develop areas for growth</label>
      <label><input type="checkbox" name="learningOutcomes" value="Demonstrate that challenges have been undertaken, developing new skills in the process"> Demonstrate that challenges have been undertaken, developing new skills in the process</label>
      <label><input type="checkbox" name="learningOutcomes" value="Demonstrate how to initiate and plan a CAS experience"> Demonstrate how to initiate and plan a CAS experience</label>
      <label><input type="checkbox" name="learningOutcomes" value="Show commitment to and perseverance in CAS experiences"> Show commitment to and perseverance in CAS experiences</label>
      <label><input type="checkbox" name="learningOutcomes" value="Demonstrate the skills and recognise the benefits of working collaboratively"> Demonstrate the skills and recognise the benefits of working collaboratively</label>
      <label><input type="checkbox" name="learningOutcomes" value="Demonstrate engagement with issues of global significance"> Demonstrate engagement with issues of global significance</label>
      <label><input type="checkbox" name="learningOutcomes" value="Recognise and consider the ethics of choices and actions"> Recognise and consider the ethics of choices and actions</label>
    </div>

    <!-- Reflection -->
    <label>Personal Reflection</label>
    <textarea name="reflection" rows="6" placeholder="What did I do? What did I learn about myself and others? How did I feel before, during, and after the activity? Did I face challenges, and how did I overcome them? How does this activity contribute to my personal growth and goals?" required></textarea>

    <!-- Hours Logged -->
    <label>Hours Logged</label>
    <div style="display: flex; gap: 10px;">
      <div><strong>Creativity:</strong><br><input type="number" name="creativityHours" min="0"></div>
      <div><strong>Action:</strong><br><input type="number" name="actionHours" min="0"></div>
      <div><strong>Service:</strong><br><input type="number" name="serviceHours" min="0"></div>
    </div>

    <button type="submit">Submit</button>
<div id="toast">✅ Your CAS activity has been submitted successfully!</div>

  </form>

  <script>
  const scriptURL = "https://script.google.com/macros/s/AKfycbxC_981gm8HedrJLdDtKccF1UFiVxGZsl1zuoXGuj-TBzamtm2P7M7ravEydFS-OZKJZQ/exec";
  const form = document.getElementById("casForm");
  const toast = document.getElementById("toast");

  form.addEventListener("submit", e => {
    e.preventDefault();

    const data = Object.fromEntries(new FormData(form).entries());

    fetch(scriptURL, {
      method: "POST",
      body: JSON.stringify(data)
    })
    .then(res => {
      if (res.ok) {
        showToast("✅ Your CAS activity has been submitted successfully!", "#00ff7f");
        form.reset();
      } else {
        showToast("⚠️ Server error. Please try again.", "#ffcc00");
      }
    })
    .catch(err => {
      console.error(err);
      showToast("❌ Network error. Please check your connection.", "#ff4444");
    });
  });

  function showToast(message, color) {
    toast.textContent = message;
    toast.style.color = color;
    toast.classList.add("show");

    setTimeout(() => {
      toast.classList.remove("show");
    }, 4000);
  }
</script>



</body>
</html>
