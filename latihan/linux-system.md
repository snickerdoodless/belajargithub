### Interactive Quiz

#### Question 1: What is the capital of France?

<ul>
  <li><input type="radio" id="q1-a" name="q1"> Paris</li>
  <li><input type="radio" id="q1-b" name="q1"> Berlin</li>
  <li><input type="radio" id="q1-c" name="q1"> London</li>
</ul>

<div id="q1-feedback"></div>

#### Question 2: What is the largest planet in our solar system?

<ul>
  <li><input type="radio" id="q2-a" name="q2"> Earth</li>
  <li><input type="radio" id="q2-b" name="q2"> Saturn</li>
  <li><input type="radio" id="q2-c" name="q2"> Jupiter</li>
</ul>

<div id="q2-feedback"></div>

#### Reset Button

<button id="reset-btn">Reset Quiz</button>

<!-- Hide JavaScript code -->
<script style="display: none;">
  // Question 1 feedback
  document.querySelectorAll("input[name='q1']").forEach(function(radio) {
    radio.addEventListener("click", function() {
      if (radio.id === "q1-a") {
        document.getElementById("q1-feedback").innerHTML = "<span style='color: green;'>Correct!</span>";
      } else {
        document.getElementById("q1-feedback").innerHTML = "<span style='color: red;'>Incorrect. The correct answer is Paris.</span>";
      }
    });
  });

  // Question 2 feedback
  document.querySelectorAll("input[name='q2']").forEach(function(radio) {
    radio.addEventListener("click", function() {
      if (radio.id === "q2-c") {
        document.getElementById("q2-feedback").innerHTML = "<span style='color: green;'>Correct!</span>";
      } else {
        document.getElementById("q2-feedback").innerHTML = "<span style='color: red;'>Incorrect. The correct answer is Jupiter.</span>";
      }
    });
  });

  // Reset button functionality
  document.getElementById("reset-btn").addEventListener("click", function() {
    // Reset radio buttons
    document.querySelectorAll("input[type='radio']").forEach(function(radio) {
      radio.checked = false;
    });
    // Reset feedback
    document.getElementById("q1-feedback").innerHTML = "";
    document.getElementById("q2-feedback").innerHTML = "";
  });
</script>
