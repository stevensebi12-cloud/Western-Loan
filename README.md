export default function WesternLoan() { const loanOptions = [5000, 10000, 15000, 20000];

return ( <div className="min-h-screen bg-gradient-to-b from-blue-100 to-white p-4"> <div className="max-w-5xl mx-auto grid md:grid-cols-2 gap-6"> <div className="bg-white rounded-[2rem] shadow-2xl p-6"> <div className="text-center mb-6"> <div className="mx-auto w-24 h-24 bg-blue-700 rounded-full flex items-center justify-center text-white text-3xl font-bold shadow-lg">WL</div> <h1 className="text-4xl font-bold text-blue-700 mt-3">Western Loan</h1> <p className="text-gray-500">Quick • Simple • Secure</p> </div>

<div className="bg-blue-700 text-white rounded-3xl p-5 mb-5 text-center">
        <h2 className="text-2xl font-bold">Apply For A Loan</h2>
        <p>Get approved from Ksh 5,000 instantly</p>
      </div>

      <div className="space-y-3">
        <input type="text" placeholder="Full Name" className="w-full border rounded-2xl p-3" />
        <input type="tel" placeholder="Phone Number" className="w-full border rounded-2xl p-3" />
        <input type="password" placeholder="Password" className="w-full border rounded-2xl p-3" />
        <button className="w-full bg-blue-700 text-white py-3 rounded-2xl font-semibold">Login</button>
        <button className="w-full border border-blue-700 text-blue-700 py-3 rounded-2xl font-semibold">Create Account</button>
      </div>

      <div className="bg-blue-50 rounded-3xl p-4 mt-5">
        <h2 className="font-bold text-center mb-3">Approved Loan Limits</h2>
        <div className="grid grid-cols-2 gap-3">
          {loanOptions.map((amount) => (
            <button key={amount} className="bg-white rounded-2xl p-3 shadow font-bold text-blue-700">
              Ksh {amount.toLocaleString()}
            </button>
          ))}
        </div>
      </div>
    </div>

    <div className="space-y-5">
      <div className="bg-white rounded-[2rem] shadow-xl p-5">
        <h2 className="text-xl font-bold text-center mb-3">Customer Dashboard</h2>
        <div className="space-y-2 text-gray-700">
          <p><strong>Account Status:</strong> Active</p>
          <p><strong>Approved Limit:</strong> Ksh 5,000</p>
          <p><strong>Loan Status:</strong> No Active Loan</p>
          <p><strong>Balance:</strong> Ksh 0</p>
        </div>
      </div>

      <div className="bg-green-50 rounded-[2rem] p-5 border shadow-sm">
        <h2 className="font-bold text-center text-green-700">SMS Verification</h2>
        <input type="text" placeholder="Enter SMS Code" className="w-full border rounded-2xl p-3 mt-3" />
        <button className="w-full bg-green-600 text-white py-3 rounded-2xl mt-3">Verify Code</button>
      </div>

      <div className="bg-white rounded-[2rem] shadow-xl p-5 border">
        <h2 className="font-bold text-center text-green-700 mb-2">M-Pesa Payment</h2>
        <p className="text-sm text-gray-500 text-center mb-3">Secure payment page style</p>
        <input type="tel" placeholder="M-Pesa Number" className="w-full border rounded-2xl p-3 mb-3" />
        <button className="w-full bg-green-600 text-white py-3 rounded-2xl font-semibold">Pay Now</button>
      </div>

      <div className="bg-white rounded-[2rem] p-5 shadow-xl text-center">
        <h2 className="font-bold mb-3">WhatsApp Support</h2>
        <a href="https://wa.me/254720088958" className="bg-green-500 text-white px-5 py-3 rounded-2xl inline-block font-semibold">
          Chat: 0720088958
        </a>
      </div>

      <div className="bg-white rounded-[2rem] p-5 shadow-xl text-sm text-gray-600">
        <h2 className="font-bold text-lg mb-2">Terms & Conditions</h2>
        <p>Loans are subject to verification and approval. Users should review repayment terms before accepting a loan.</p>
        <h2 className="font-bold text-lg mt-4 mb-2">Privacy Policy</h2>
        <p>Your account information is protected and used only to provide services on Western Loan.</p>
      </div>
    </div>
  </div>
</div>

); }export default function WesternLoan() {# Western-Loan