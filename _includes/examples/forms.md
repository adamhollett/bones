## Forms

Forms have basic, accessible styles.

<form>
  <label>
    Name
    <input type="text" id="name" name="name">
  </label>

  <label>
    Email
    <input type="text" id="email" name="email" required>
  </label>

  <label>
    Age range
    <select>
      <option value="0–10">0–10</option>
      <option value="11–20">11–20</option>
      <option value="21–30">21–30</option>
      <option value="31–40">31–40</option>
      <option value="41–50">41–50</option>
      <option value="50+">50+</option>
    </select>
  </label>

  <label>
    Message
    <textarea id="message" name="message" required></textarea>
  </label>

  <button type="submit">Submit</button>
</form>
