<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>مدرب اللياقة الذكي</title>
  <script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
  <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
  <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background: #f0f4f8; display: flex; justify-content: center; padding: 20px; }
    #root { width: 100%; max-width: 600px; }
    .app > div { background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin-bottom: 20px; }
    label { display: block; margin: 12px 0 5px; font-weight: bold; color: #2c3e50; }
    input, select, button { width: 100%; padding: 12px; margin: 5px 0 15px; border: 1px solid #ddd; border-radius: 8px; font-size: 16px; }
    button { background: #3498db; color: white; border: none; cursor: pointer; font-weight: bold; transition: background 0.3s; }
    button:hover { background: #2980b9; }
    button:disabled { background: #95a5a6; cursor: not-allowed; }
    fieldset { border: 1px solid #ddd; border-radius: 8px; padding: 15px; margin: 15px 0; }
    legend { font-weight: bold; padding: 0 10px; }
    .exercise-item { display: flex; justify-content: space-between; align-items: center; background: #e8f0fe; padding: 10px; border-radius: 8px; margin: 10px 0; }
    .video-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 15px 0; border-radius: 8px; }
    .video-container iframe { position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0; }
    .dashboard h2, .dashboard h3 { margin-bottom: 10px; color: #2c3e50; }
    .actions { display: flex; gap: 10px; margin-top: 20px; }
    .actions button { flex: 1; }
    .session-finish select { margin: 10px 0; }
  </style>
</head>
<body>
  <div id="root"></div>
  <script type="text/babel">
    const { useState, useEffect } = React;

    // ======================== البيانات الثابتة ========================
    const exercises = [
      { id: 1, name: 'Squats', nameAr: 'القرفصاء', muscleGroup: 'legs', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/aclHkVaku9U' },
      { id: 2, name: 'Lunges', nameAr: 'الاندفاع', muscleGroup: 'legs', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/QOVaHwm-Q6U' },
      { id: 3, name: 'Push-ups', nameAr: 'تمارين الضغط', muscleGroup: 'chest', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/IODxDxX7oi4' },
      { id: 4, name: 'Knee Push-ups', nameAr: 'ضغط الركبة', muscleGroup: 'chest', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/jWcDvq7rGM4' },
      { id: 5, name: 'Plank', nameAr: 'اللوح الخشبي', muscleGroup: 'core', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/pSHjTRCQxIw' },
      { id: 6, name: 'Glute Bridge', nameAr: 'جسر الألوية', muscleGroup: 'glutes', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/wPM8icPu6H8' },
      { id: 7, name: 'Standing Calf Raises', nameAr: 'رفع السمانة واقفاً', muscleGroup: 'calves', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/3UWi44yN-wM' },
      { id: 8, name: 'Jumping Jacks', nameAr: 'قفز الحبل', muscleGroup: 'cardio', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 60, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/c4DAnQ6DtF8' },
      { id: 9, name: 'High Knees', nameAr: 'الركب العالية', muscleGroup: 'cardio', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 60, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/8opcQdC-V-U' },
      { id: 10, name: 'Dumbbell Shoulder Press', nameAr: 'ضغط الكتف بالدمبل', muscleGroup: 'shoulders', difficulty: 'intermediate', equipment: ['dumbbell'], minAge: 16, maxAge: 80, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/qEwKCR5JCog' },
      { id: 11, name: 'Dumbbell Row', nameAr: 'سحب الدمبل', muscleGroup: 'back', difficulty: 'intermediate', equipment: ['dumbbell'], minAge: 16, maxAge: 80, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/roCP6wCXPqo' },
      { id: 12, name: 'Dumbbell Squat', nameAr: 'قرفصاء بالدمبل', muscleGroup: 'legs', difficulty: 'intermediate', equipment: ['dumbbell'], minAge: 16, maxAge: 80, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/1oed-UmAxFs' },
      { id: 13, name: 'Bicycle Crunches', nameAr: 'بطن الدراجة', muscleGroup: 'core', difficulty: 'intermediate', equipment: ['none'], minAge: 13, maxAge: 80, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/9FGilxCbdz8' },
      { id: 14, name: 'Wall Sit', nameAr: 'الجلوس على الحائط', muscleGroup: 'legs', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/y-wV4VenR3w' },
      { id: 15, name: 'Leg Raises', nameAr: 'رفع الساقين', muscleGroup: 'core', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/JB2oyawG9KI' },
      { id: 16, name: 'Chair Squats', nameAr: 'قرفصاء الكرسي', muscleGroup: 'legs', difficulty: 'beginner', equipment: ['none'], minAge: 60, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/2_3kDk7z1UU' },
      { id: 17, name: 'Standing Side Leg Raise', nameAr: 'رفع الساق جانباً', muscleGroup: 'legs', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/dK_n5KZ6YJI' },
      { id: 18, name: 'Yoga Child’s Pose', nameAr: 'وضعية الطفل', muscleGroup: 'stretching', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/2MJGg-dUKh0' },
      { id: 19, name: 'Cat-Cow Stretch', nameAr: 'تمدد القطة والبقرة', muscleGroup: 'stretching', difficulty: 'beginner', equipment: ['none'], minAge: 13, maxAge: 100, genderPreference: 'all', videoUrl: 'https://www.youtube.com/embed/kqnua4rHVVA' },
      { id: 20, name: 'Kegel Exercises', nameAr: 'تمارين قاع الحوض', muscleGroup: 'pelvic', difficulty: 'beginner', equipment: ['none'], minAge: 18, maxAge: 100, genderPreference: 'female', videoUrl: 'https://www.youtube.com/embed/10GgQ5IfcMk' },
    ];

    const planTemplates = [
      {
        id: 1,
        name: 'Full Body Beginner',
        goal: 'general_fitness',
        level: 'beginner',
        durationWeeks: 4,
        weeksData: {
          week1: [
            { exerciseIds: [1,4,5,8,18], reps: [10,8,30,30,30], rest: 60 },
            { exerciseIds: [2,15,7,9,19], reps: [8,10,12,30,30], rest: 60 },
          ],
          week2: [
            { exerciseIds: [1,3,5,8,18], reps: [12,8,35,35,30], rest: 55 },
            { exerciseIds: [2,6,7,9,19], reps: [10,12,12,30,30], rest: 55 },
          ],
          week3: [
            { exerciseIds: [1,4,5,14,8], reps: [12,10,40,30,40], rest: 50 },
            { exerciseIds: [2,15,7,9,13], reps: [10,12,15,40,20], rest: 50 },
          ],
          week4: [
            { exerciseIds: [1,3,5,14,9], reps: [15,10,45,35,45], rest: 45 },
            { exerciseIds: [2,6,7,13,19], reps: [12,15,15,25,30], rest: 45 },
          ],
        },
      },
      {
        id: 2,
        name: 'Strength Intermediate',
        goal: 'muscle_build',
        level: 'intermediate',
        durationWeeks: 4,
        weeksData: {
          week1: [
            { exerciseIds: [10,11,12,13], reps: [10,10,8,15], rest: 45 },
            { exerciseIds: [10,11,6,13], reps: [10,10,12,15], rest: 45 },
          ],
          week2: [
            { exerciseIds: [10,11,12,5], reps: [12,12,10,40], rest: 40 },
            { exerciseIds: [10,11,3,13], reps: [12,12,10,20], rest: 40 },
          ],
          week3: [
            { exerciseIds: [10,11,12,13], reps: [14,14,12,20], rest: 35 },
            { exerciseIds: [10,11,6,5], reps: [14,14,15,45], rest: 35 },
          ],
          week4: [
            { exerciseIds: [10,11,12,13], reps: [16,16,14,25], rest: 30 },
            { exerciseIds: [10,11,3,5], reps: [16,16,12,50], rest: 30 },
          ],
        },
      },
    ];

    // ======================== دوال مساعدة للتخزين ========================
    const PROFILE_KEY = 'fitness_profile';
    const PLAN_KEY = 'fitness_user_plan';
    const LOG_KEY = 'fitness_workout_log';

    const loadFromStorage = (key, fallback = null) => {
      try {
        const item = localStorage.getItem(key);
        return item ? JSON.parse(item) : fallback;
      } catch { return fallback; }
    };
    const saveToStorage = (key, value) => localStorage.setItem(key, JSON.stringify(value));

    // ======================== دالة توليد الخطة ========================
    function generatePlan(profile) {
      const { age, gender, goal, level, weeklyDays, sessionDuration, equipment } = profile;
      
      // تصفية التمارين المناسبة
      const suitableExercises = exercises.filter(ex => {
        if (ex.minAge && age < ex.minAge) return false;
        if (ex.maxAge && age > ex.maxAge) return false;
        if (ex.genderPreference !== 'all' && ex.genderPreference !== gender) return false;
        if (ex.equipment && ex.equipment.length > 0 && !ex.equipment.includes('none')) {
          const hasAll = ex.equipment.every(eq => equipment.includes(eq));
          if (!hasAll) return false;
        }
        return true;
      });

      // اختيار القالب المناسب
      let template = planTemplates.find(t => t.goal === goal && t.level === level);
      if (!template) {
        template = planTemplates.find(t => t.goal === goal) || planTemplates[0];
      }

      const weeksData = {};
      const weekKeys = Object.keys(template.weeksData).slice(0, template.durationWeeks);
      
      weekKeys.forEach((weekKey, idx) => {
        const weekDays = [];
        const daysData = template.weeksData[weekKey];
        for (let i = 0; i < weeklyDays; i++) {
          const dayTemplate = daysData[i % daysData.length];
          const exercisesForDay = dayTemplate.exerciseIds.map(id => {
            let ex = suitableExercises.find(e => e.id === id);
            if (!ex) {
              const original = exercises.find(e => e.id === id);
              if (original) {
                ex = suitableExercises.find(e => e.muscleGroup === original.muscleGroup && e.difficulty === original.difficulty);
              }
            }
            return ex || suitableExercises[0];
          });
          weekDays.push({
            exercises: exercisesForDay,
            reps: dayTemplate.reps,
            rest: dayTemplate.rest,
            duration: sessionDuration
          });
        }
        weeksData[`week${idx + 1}`] = weekDays;
      });

      return {
        startDate: new Date().toISOString().split('T')[0],
        endDate: new Date(Date.now() + template.durationWeeks * 7 * 24 * 60 * 60 * 1000).toISOString().split('T')[0],
        weeksData,
        currentWeek: 1,
        adaptationLog: []
      };
    }

    // ======================== مكونات التطبيق ========================
    function Onboarding({ onComplete }) {
      const [name, setName] = useState('');
      const [gender, setGender] = useState('male');
      const [age, setAge] = useState(25);
      const [goal, setGoal] = useState('general_fitness');
      const [weeklyDays, setWeeklyDays] = useState(3);
      const [equipment, setEquipment] = useState(['none']);

      const toggleEquipment = (item) => {
        if (equipment.includes(item)) {
          setEquipment(equipment.filter(e => e !== item));
        } else {
          setEquipment([...equipment, item]);
        }
        if (equipment.length === 1 && equipment[0] === 'none' && item !== 'none') {
          setEquipment(equipment.filter(e => e !== 'none'));
        }
        if (equipment.length === 0) setEquipment(['none']);
      };

      const handleSubmit = (e) => {
        e.preventDefault();
        const profile = {
          name,
          gender,
          age: Number(age),
          goal,
          level: age > 55 || age < 18 ? 'beginner' : 'beginner',
          weeklyDays: Number(weeklyDays),
          sessionDuration: 30,
          equipment,
        };
        saveToStorage(PROFILE_KEY, profile);
        onComplete(profile);
      };

      return (
        <div className="onboarding-container">
          <h1>مرحباً بك في مدربك الذكي</h1>
          <form onSubmit={handleSubmit}>
            <label>الاسم</label>
            <input value={name} onChange={e => setName(e.target.value)} required />
            <label>الجنس</label>
            <select value={gender} onChange={e => setGender(e.target.value)}>
              <option value="male">ذكر</option>
              <option value="female">أنثى</option>
              <option value="other">آخر</option>
            </select>
            <label>العمر</label>
            <input type="number" value={age} onChange={e => setAge(e.target.value)} min="13" max="100" />
            <label>الهدف</label>
            <select value={goal} onChange={e => setGoal(e.target.value)}>
              <option value="general_fitness">لياقة عامة</option>
              <option value="weight_loss">خسارة وزن</option>
              <option value="muscle_build">بناء عضلات</option>
            </select>
            <label>أيام التمرين في الأسبوع</label>
            <select value={weeklyDays} onChange={e => setWeeklyDays(e.target.value)}>
              {[2,3,4,5,6].map(d => <option key={d} value={d}>{d}</option>)}
            </select>
            <fieldset>
              <legend>المعدات المتوفرة</legend>
              <label><input type="checkbox" checked={equipment.includes('none')} onChange={() => toggleEquipment('none')} /> بدون معدات</label>
              <label><input type="checkbox" checked={equipment.includes('dumbbell')} onChange={() => toggleEquipment('dumbbell')} /> دمبل</label>
              <label><input type="checkbox" checked={equipment.includes('mat')} onChange={() => toggleEquipment('mat')} /> سجادة</label>
              <label><input type="checkbox" checked={equipment.includes('resistance_band')} onChange={() => toggleEquipment('resistance_band')} /> شريط مقاومة</label>
            </fieldset>
            <button type="submit">ابدأ رحلتك</button>
          </form>
        </div>
      );
    }

    function Dashboard({ profile, plan, log, onStartSession, onLibrary, onReset }) {
      if (!plan) return <div>جاري تحضير خطتك...</div>;

      const currentWeek = plan.currentWeek;
      const weekKey = `week${currentWeek}`;
      const daysThisWeek = plan.weeksData[weekKey] || [];
      const todayWorkout = daysThisWeek.length > 0 ? daysThisWeek[0] : null;

      return (
        <div className="dashboard">
          <h2>مرحباً {profile.name}!</h2>
          <p>الأسبوع {currentWeek} من {Object.keys(plan.weeksData).length} أسابيع</p>
          <p>الجلسات المكتملة: {log.length}</p>
          {todayWorkout ? (
            <div>
              <h3>تمرين اليوم</h3>
              {todayWorkout.exercises.map((ex, idx) => (
                <div key={ex.id} className="exercise-item">
                  <span>{ex.nameAr || ex.name}</span>
                  <span>{todayWorkout.reps[idx] ? `${todayWorkout.reps[idx]} عدة` : 'حسب الزمن'}</span>
                </div>
              ))}
              <button onClick={onStartSession}>ابدأ الجلسة</button>
            </div>
          ) : <p>لا يوجد تمرين اليوم.</p>}
          <div className="actions">
            <button onClick={onLibrary}>مكتبة التمارين</button>
            <button onClick={onReset}>تغيير الخطة (حذف البيانات)</button>
          </div>
        </div>
      );
    }

    function WorkoutSession({ plan, onFinish, onBack }) {
      const currentWeek = `week${plan.currentWeek}`;
      const dayWorkout = plan.weeksData[currentWeek]?.[0] || { exercises: [], reps: [] };
      const exercisesList = dayWorkout.exercises;
      const [currentStep, setCurrentStep] = useState(0);
      const [feedback, setFeedback] = useState('');
      const [completed, setCompleted] = useState(false);

      const currentExercise = exercisesList[currentStep];

      const next = () => {
        if (currentStep < exercisesList.length - 1) setCurrentStep(currentStep + 1);
        else setCompleted(true);
      };

      const finish = () => {
        const sessionData = {
          date: new Date().toISOString().split('T')[0],
          exercises: exercisesList.map(ex => ex.id),
          feedback,
        };
        onFinish(sessionData);
      };

      if (completed) {
        return (
          <div className="session-finish">
            <h3>أحسنت! لقد أكملت التمرين.</h3>
            <p>كيف كانت شدة التمرين؟</p>
            <select value={feedback} onChange={e => setFeedback(e.target.value)}>
              <option value="">اختر...</option>
              <option value="easy">سهل</option>
              <option value="just_right">مناسب</option>
              <option value="hard">صعب</option>
            </select>
            <button onClick={finish} disabled={!feedback}>إنهاء وحفظ</button>
            <button onClick={onBack}>رجوع دون حفظ</button>
          </div>
        );
      }

      return (
        <div className="session">
          <h2>جلسة التمرين</h2>
          {currentExercise && (
            <div>
              <h3>{currentExercise.nameAr || currentExercise.name}</h3>
              <div className="video-container">
                <iframe src={currentExercise.videoUrl} title={currentExercise.name} allowFullScreen></iframe>
              </div>
              <p>التكرارات: {dayWorkout.reps[currentStep] || 'حسب الإحساس'}</p>
              <button onClick={next}>
                {currentStep < exercisesList.length - 1 ? 'التمرين التالي' : 'إنهاء الجلسة'}
              </button>
            </div>
          )}
          <button onClick={onBack}>إنهاء مبكراً</button>
        </div>
      );
    }

    function Library({ onBack }) {
      return (
        <div className="library">
          <button onClick={onBack}>رجوع</button>
          <h2>مكتبة التمارين</h2>
          {exercises.map(ex => (
            <div key={ex.id} className="exercise-item" style={{flexDirection: 'column', alignItems: 'flex-start'}}>
              <strong>{ex.nameAr || ex.name}</strong>
              <small>العضلة: {ex.muscleGroup} | المستوى: {ex.difficulty}</small>
              <a href={ex.videoUrl} target="_blank" rel="noopener noreferrer">شاهد الفيديو</a>
            </div>
          ))}
        </div>
      );
    }

    function App() {
      const [profile, setProfile] = useState(() => loadFromStorage(PROFILE_KEY));
      const [plan, setPlan] = useState(() => loadFromStorage(PLAN_KEY));
      const [log, setLog] = useState(() => loadFromStorage(LOG_KEY, []));
      const [screen, setScreen] = useState('dashboard'); // 'dashboard', 'session', 'library'

      useEffect(() => {
        if (profile && !plan) {
          const newPlan = generatePlan(profile);
          setPlan(newPlan);
          saveToStorage(PLAN_KEY, newPlan);
        }
      }, [profile, plan]);

      useEffect(() => { if (profile) saveToStorage(PROFILE_KEY, profile); }, [profile]);
      useEffect(() => { if (plan) saveToStorage(PLAN_KEY, plan); }, [plan]);
      useEffect(() => { saveToStorage(LOG_KEY, log); }, [log]);

      const handleCompleteOnboarding = (newProfile) => {
        setProfile(newProfile);
        setPlan(null); // trigger regeneration
        setScreen('dashboard');
      };

      const startSession = () => setScreen('session');
      const finishSession = (sessionData) => {
        setLog([...log, sessionData]);
        setScreen('dashboard');
      };
      const showLibrary = () => setScreen('library');
      const backToDashboard = () => setScreen('dashboard');
      const resetAll = () => {
        if (confirm('هل أنت متأكد من حذف جميع البيانات والبدء من جديد؟')) {
          localStorage.clear();
          setProfile(null);
          setPlan(null);
          setLog([]);
          setScreen('dashboard');
        }
      };

      if (!profile) {
        return <Onboarding onComplete={handleCompleteOnboarding} />;
      }

      return (
        <div className="app">
          {screen === 'dashboard' && (
            <Dashboard
              profile={profile}
              plan={plan}
              log={log}
              onStartSession={startSession}
              onLibrary={showLibrary}
              onReset={resetAll}
            />
          )}
          {screen === 'session' && (
            <WorkoutSession plan={plan} onFinish={finishSession} onBack={backToDashboard} />
          )}
          {screen === 'library' && (
            <Library onBack={backToDashboard} />
          )}
        </div>
      );
    }

    ReactDOM.createRoot(document.getElementById('root')).render(<App />);
  </script>
</body>
</html>
