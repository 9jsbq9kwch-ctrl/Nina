import { useState } from "react";

export default function App() {
  const [message, setMessage] = useState("");

  function showMessage() {
    setMessage("🔥 أنا أصبحت أتعلم React!");
  }

  return (
    <div style={{ textAlign: "center", marginTop: "50px" }}>
      <h1>مرحبا بيك في React 😈</h1>

      <button onClick={showMessage}>
        اضغط هنا
      </button>

      <p>{message}</p>
    </div>
  );
}
